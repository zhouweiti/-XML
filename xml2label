#coding = utf-8

import xml.etree.cElementTree as et
import os
root_dir = 'D:/tilda_CD1+CD2/tilda_CD1+CD2/xmldata/'
list = os.listdir(root_dir)
for i in list:
    # f = open(root_dir+i)
    tree = et.parse(root_dir+i)
    root = tree.getroot()
    # filename = root.find('filename').text
    # print(filename)
    for Object in root.findall('object'):
        name = Object.find('name').text
        print(name)
        bndbox = Object.find('bndbox')
        xmin = bndbox.find('xmin').text
        ymin = bndbox.find('ymin').text
        xmax = bndbox.find('xmax').text
        ymax = bndbox.find('ymax').text
        print(xmin, ymin, xmax, ymax)


