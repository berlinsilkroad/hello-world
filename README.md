# hello-world
%画出左旋圆和右旋圆
clc,clear;
for i=-5:0.01:5
y=sqrt(25-i^2)+5;%画圆点
hold on;
plot(i,y,'.','markersize',18)
end
for i=-5:0.01:5
y=-sqrt(25-i^2)+5;
hold on; 
plot(i,y,'.','markersize',18)
end
for i=-5:0.01:5
y=sqrt(25-i^2)-5;
hold on;
plot(i,y,'.','markersize',18)
end
for i=-5:0.01:5
y=-sqrt(25-i^2)-5;
hold on;
plot(i,y,'.','markersize',18)
end


%画出迭代点
for j=-3.1415926:0.1:3.1415926
 x=5*sin(j)+cos(j)*(40-j*5);%迭代出扩大范围的x的坐标
 y=5*(-cos(j)+1)+sin(j)*(40-j*5)-10;%迭代出扩大范围的y的坐标
 plot(x,y,'.','markersize',18)
 hold on;
end
hold off
for j=-3.1415926:0.1:3.1415926
 x=5*sin(j)+cos(j)*(40-j*5);%迭代出扩大范围的x的坐标
 y=-(5*(-cos(j)+1)+sin(j)*(40-j*5)-10);%迭代出扩大范围的y的坐标
 plot(x,y,'.','markersize',18)
 hold on;
end
