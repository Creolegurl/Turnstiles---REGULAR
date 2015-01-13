df = df[df['DESCn'] == 'REGULAR'] # Filter by REGULAR  
df['ENTRIESn_hourly'] = (df['ENTRIESn'] - df['ENTRIESn'].shift(1)).fillna(1)
