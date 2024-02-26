# trade-bot-rsi
RSI 80/20
import random

class TradeBot:
    def __init__(self):
        self.rsi_threshold_overbought = 80
        self.rsi_threshold_oversold = 20

    def calculate_rsi(self, prices, period=14):
        # Tính toán chỉ báo RSI
        # (Đoạn mã này chỉ là một đoạn mã giả định và không hoàn chỉnh)
        return random.randint(0, 100)

    def is_overbought(self, rsi_value):
        return rsi_value > self.rsi_threshold_overbought

    def is_oversold(self, rsi_value):
        return rsi_value < self.rsi_threshold_oversold

    def trade_decision(self, rsi_value):
        if self.is_overbought(rsi_value):
            return "Sell"
        elif self.is_oversold(rsi_value):
            return "Buy"
        else:
            return "Hold"

# Sử dụng trade bot
if __name__ == "__main__":
    bot = TradeBot()
    historical_prices = [random.randint(50, 100) for _ in range(30)]

    current_rsi = bot.calculate_rsi(historical_prices)
    decision = bot.trade_decision(current_rsi)

    print(f"Current RSI: {current_rsi}")
    print(f"Trade Decision: {decision}")
