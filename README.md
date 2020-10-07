# Python-GUI-Attribute-Error
Import Area, but PyCharm reports AttributeError

import sys
from PyQt5.QtCore import pyqtSlot
from PyQt5.QtWidgets import QMainWindow, QApplication
import area

dictProvince = {2: '北京', 3: '安徽', 4: '福建', 5: '甘肃', 6: '广东', 7: '广西', 8: '贵州', 9: '海南', 10: '河北',
                11: '河南', 12: '黑龙江', 13: '湖北', 14: '湖南', 15: '吉林', 16: '江苏', 17: '江西', 18: '辽宁',
                19: '内蒙古', 20: '宁夏', 21: '青海', 22: '山东', 23: '山西', 24: '陕西', 25: '上海', 26: '四川',
                27: '天津', 28: '西藏', 29: '新疆', 30: '云南', 31: '浙江', 32: '重庆', 33: '香港', 34: '澳门',
                35: '台湾'}
def __init__(self, parent=None):
        """
     Constructor

     @param parent reference to the parent widget
     @type QWidget
     """
     super(MainWindow, self).__init__(parent)
     self.setupUi(self)
     self.comboBox.clear()  
     self.comboBox.addItem('Choose')
     for k, v in area.dictProvince.items():
         self.comboBox.addItem(v, k)  
