# Tips and Tricks

<ul>
  <li><b>Pandas library (df as a dataframe object)</b>
    <ul>
        <li><a href="https://www.kdnuggets.com/2019/11/speed-up-pandas-4x.html" target="_blank">Speed Up Pandas by 4 using Modin</a></li>
        <li><b>Column access into a pandas dataframe</b>:</li>
          <ul>
            <li><img src="https://github.com/montse-llos/data-science/blob/master/tips-and-tricks/pandas-selections-and-indexing.png"></li>
            <li>df.iloc[:,0]: all rows from column 0  </li>
            <li>df.loc[:,['ColName1']]: all rows from column 'ColName1'</li>
            <li>df[['ColName1','ColName2']]: new dataframe with 'ColName1' and 'ColName2'</li>
         </ul>
        <li>df.info() => <b>describes type of object and sizes</b></li>
        <li>df.describe() => <b>for every column, informations about average, standard deviation, etc</b> </li>
      <li><b>Delete columns</b>:</li>
        <ul>
          <li>df.drop ('Gender', axis=1, inplace=True) => deletes the column 'Gender' and updates df without 'Gender' column (because inplace=True).</li>  
          <li>df_new = df.drop (columns=['Gender','Age'], axis=1) => deletes columns 'Gender' and 'Age' and puts this modified dataframe into df_new (df stills contains Gender and Age)</li>  
        </ul>
      <li><b>Copy dataframes</b>:</li>
        <ul>
          <li>df_new = df => df_new is a reference to df (changes in df are reflected into df_new)y</li>
          <li>df_new = df.copy() => df_new is a new copy of df (changes in df are not reflected into df_new)</li>
        </ul>
      <li><b>Mapping</b>:</li>
        <ul>
          level_map = {1: 'high', 2: 'medium', 3: 'low'}  
          df['c_level'] = df['c'].map(level_map)
        </ul>  
    </ul>
  </li>
  <li><b>R</li>
    <ul>
        <li><a href="https://support.rstudio.com/hc/en-us/articles/201057987-Quick-list-of-useful-R-packages">List of useful Rpackages</a>   </li>
    </ul>
  </li>
</ul>
