import pytest
import yaml

from pythoncode.calc import Calculator

with open('./datas/calc.yml')as f:
    datas = yaml.safe_load(f)['add']
    adddatas = datas['datas']
    myid = datas['myid']
with open('./datas/calc.yml',encoding="utf-8")as f:
    datas = yaml.safe_load(f)['div']
    divdatas = datas['datas']
    myid1 = datas['myid']
class Testcalc:
    def setup_class(self):
        self.calc = Calculator()
        print("开始计算")
    def teardown_class(self):
        print("计算结束")
    @pytest.mark.parametrize('a,b,expect',adddatas,ids=myid)
    def test_add(self,a,b,expect):
        result = self.calc.add(a,b)
        assert expect == result

    @pytest.mark.parametrize('a,b,expect', divdatas, ids=myid1)
    def test_div(self,a,b,expect):
        result = self.calc.div(a,b)
        assert expect == result















