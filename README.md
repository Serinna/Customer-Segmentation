Dataset from Kaggle https://www.kaggle.com/vjchoudhary7/customer-segmentation-tutorial-in-python

Before applying K-means clustering, I scaled numerical features and explored features and their relationship. By comparing histogram and observing scatter matrix between between male and female, we can conclude that gender will not affect segmentation.

Then I applied t-SNE to visualize data. By result, there're at least 2 groups significantly separated from others. Other groups are not clearly divided, mainly due to the small amount of data.
By applying K-means and observing sum of squared distance, I finally chose k=6.

I used plotly to visualize result with 3 dimension. One of the benefit of plotly is dynamic version: it allows users to interacting with the plot by pan and rotation.

By plot, groups are not very well segmented: data is spreading instead of gathering closely, and one of the groups has outliers lying far from the group cluster. However, there's still sign of segmentation. result will be improved if we have more data.
