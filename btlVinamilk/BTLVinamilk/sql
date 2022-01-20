USE [master]
GO
/****** Object:  Database [VINAMILK]    Script Date: 1/20/2022 10:33:11 PM ******/
CREATE DATABASE [VINAMILK]
 CONTAINMENT = NONE
 ON  PRIMARY 
( NAME = N'VINAMILK', FILENAME = N'D:\SQL\PSQL\MSSQL15.SQLEXPRESS\MSSQL\DATA\VINAMILK.mdf' , SIZE = 8192KB , MAXSIZE = UNLIMITED, FILEGROWTH = 65536KB )
 LOG ON 
( NAME = N'VINAMILK_log', FILENAME = N'D:\SQL\PSQL\MSSQL15.SQLEXPRESS\MSSQL\DATA\VINAMILK_log.ldf' , SIZE = 8192KB , MAXSIZE = 2048GB , FILEGROWTH = 65536KB )
 WITH CATALOG_COLLATION = DATABASE_DEFAULT
GO
ALTER DATABASE [VINAMILK] SET COMPATIBILITY_LEVEL = 150
GO
IF (1 = FULLTEXTSERVICEPROPERTY('IsFullTextInstalled'))
begin
EXEC [VINAMILK].[dbo].[sp_fulltext_database] @action = 'enable'
end
GO
ALTER DATABASE [VINAMILK] SET ANSI_NULL_DEFAULT OFF 
GO
ALTER DATABASE [VINAMILK] SET ANSI_NULLS OFF 
GO
ALTER DATABASE [VINAMILK] SET ANSI_PADDING OFF 
GO
ALTER DATABASE [VINAMILK] SET ANSI_WARNINGS OFF 
GO
ALTER DATABASE [VINAMILK] SET ARITHABORT OFF 
GO
ALTER DATABASE [VINAMILK] SET AUTO_CLOSE OFF 
GO
ALTER DATABASE [VINAMILK] SET AUTO_SHRINK OFF 
GO
ALTER DATABASE [VINAMILK] SET AUTO_UPDATE_STATISTICS ON 
GO
ALTER DATABASE [VINAMILK] SET CURSOR_CLOSE_ON_COMMIT OFF 
GO
ALTER DATABASE [VINAMILK] SET CURSOR_DEFAULT  GLOBAL 
GO
ALTER DATABASE [VINAMILK] SET CONCAT_NULL_YIELDS_NULL OFF 
GO
ALTER DATABASE [VINAMILK] SET NUMERIC_ROUNDABORT OFF 
GO
ALTER DATABASE [VINAMILK] SET QUOTED_IDENTIFIER OFF 
GO
ALTER DATABASE [VINAMILK] SET RECURSIVE_TRIGGERS OFF 
GO
ALTER DATABASE [VINAMILK] SET  DISABLE_BROKER 
GO
ALTER DATABASE [VINAMILK] SET AUTO_UPDATE_STATISTICS_ASYNC OFF 
GO
ALTER DATABASE [VINAMILK] SET DATE_CORRELATION_OPTIMIZATION OFF 
GO
ALTER DATABASE [VINAMILK] SET TRUSTWORTHY OFF 
GO
ALTER DATABASE [VINAMILK] SET ALLOW_SNAPSHOT_ISOLATION OFF 
GO
ALTER DATABASE [VINAMILK] SET PARAMETERIZATION SIMPLE 
GO
ALTER DATABASE [VINAMILK] SET READ_COMMITTED_SNAPSHOT OFF 
GO
ALTER DATABASE [VINAMILK] SET HONOR_BROKER_PRIORITY OFF 
GO
ALTER DATABASE [VINAMILK] SET RECOVERY SIMPLE 
GO
ALTER DATABASE [VINAMILK] SET  MULTI_USER 
GO
ALTER DATABASE [VINAMILK] SET PAGE_VERIFY CHECKSUM  
GO
ALTER DATABASE [VINAMILK] SET DB_CHAINING OFF 
GO
ALTER DATABASE [VINAMILK] SET FILESTREAM( NON_TRANSACTED_ACCESS = OFF ) 
GO
ALTER DATABASE [VINAMILK] SET TARGET_RECOVERY_TIME = 60 SECONDS 
GO
ALTER DATABASE [VINAMILK] SET DELAYED_DURABILITY = DISABLED 
GO
ALTER DATABASE [VINAMILK] SET ACCELERATED_DATABASE_RECOVERY = OFF  
GO
ALTER DATABASE [VINAMILK] SET QUERY_STORE = OFF
GO
USE [VINAMILK]
GO
/****** Object:  Table [dbo].[DMSUA]    Script Date: 1/20/2022 10:33:11 PM ******/
SET ANSI_NULLS ON
GO
SET QUOTED_IDENTIFIER ON
GO
CREATE TABLE [dbo].[DMSUA](
	[IDDM] [nchar](10) NOT NULL,
	[TenDM] [nvarchar](20) NULL,
	[AnhDM] [varchar](50) NULL,
 CONSTRAINT [PK_DMSUA] PRIMARY KEY CLUSTERED 
(
	[IDDM] ASC
)WITH (PAD_INDEX = OFF, STATISTICS_NORECOMPUTE = OFF, IGNORE_DUP_KEY = OFF, ALLOW_ROW_LOCKS = ON, ALLOW_PAGE_LOCKS = ON, OPTIMIZE_FOR_SEQUENTIAL_KEY = OFF) ON [PRIMARY]
) ON [PRIMARY]
GO
/****** Object:  Table [dbo].[SUA]    Script Date: 1/20/2022 10:33:11 PM ******/
SET ANSI_NULLS ON
GO
SET QUOTED_IDENTIFIER ON
GO
CREATE TABLE [dbo].[SUA](
	[ID] [int] IDENTITY(1,1) NOT NULL,
	[TieuDe] [nvarchar](50) NULL,
	[AnhBia] [nvarchar](50) NULL,
	[SoLuong] [int] NULL,
	[GiaBan] [money] NULL,
	[Mota] [ntext] NULL,
	[IDDM] [nchar](10) NULL,
 CONSTRAINT [PK_SUA] PRIMARY KEY CLUSTERED 
(
	[ID] ASC
)WITH (PAD_INDEX = OFF, STATISTICS_NORECOMPUTE = OFF, IGNORE_DUP_KEY = OFF, ALLOW_ROW_LOCKS = ON, ALLOW_PAGE_LOCKS = ON, OPTIMIZE_FOR_SEQUENTIAL_KEY = OFF) ON [PRIMARY]
) ON [PRIMARY] TEXTIMAGE_ON [PRIMARY]
GO
/****** Object:  Table [dbo].[TAIKHOAN]    Script Date: 1/20/2022 10:33:11 PM ******/
SET ANSI_NULLS ON
GO
SET QUOTED_IDENTIFIER ON
GO
CREATE TABLE [dbo].[TAIKHOAN](
	[Ten] [nchar](10) NOT NULL,
	[MatKhau] [nchar](10) NULL,
	[QuenTC] [nchar](10) NULL,
 CONSTRAINT [PK_TAIKHOAN] PRIMARY KEY CLUSTERED 
(
	[Ten] ASC
)WITH (PAD_INDEX = OFF, STATISTICS_NORECOMPUTE = OFF, IGNORE_DUP_KEY = OFF, ALLOW_ROW_LOCKS = ON, ALLOW_PAGE_LOCKS = ON, OPTIMIZE_FOR_SEQUENTIAL_KEY = OFF) ON [PRIMARY]
) ON [PRIMARY]
GO
INSERT [dbo].[DMSUA] ([IDDM], [TenDM], [AnhDM]) VALUES (N'DM1       ', N'Sữa bột vinamilk', N'dm1.jpg')
INSERT [dbo].[DMSUA] ([IDDM], [TenDM], [AnhDM]) VALUES (N'DM2       ', N'Sữa đặc', N'dm2.jpg')
INSERT [dbo].[DMSUA] ([IDDM], [TenDM], [AnhDM]) VALUES (N'DM3       ', N'Sữa đậu nành', N'dm3.jpg')
INSERT [dbo].[DMSUA] ([IDDM], [TenDM], [AnhDM]) VALUES (N'DM4       ', N'Sữa nước', N'dm4.jpg')
INSERT [dbo].[DMSUA] ([IDDM], [TenDM], [AnhDM]) VALUES (N'DM5       ', N'Sữa chua vinamilk', N'dm5.jpg')
GO
SET IDENTITY_INSERT [dbo].[SUA] ON 

INSERT [dbo].[SUA] ([ID], [TieuDe], [AnhBia], [SoLuong], [GiaBan], [Mota], [IDDM]) VALUES (1, N'Dielac Mama Gold', N'm666.jpg', 100, 250000.0000, N'Với hương vị thơm ngon và phù hợp với khẩu vị của mẹ trong giai đoạn mang thai, sữa bột Dielac Mama Gold bổ sung Sắt, Canxi, chất xơ hòa tan thế hệ mới Sc-FOS, I-ốt giúp tăng cường sức khỏe cho mẹ. Đặc biệt, sản phẩm còn bổ sung DHA, Axit Folic, Canxi hỗ trợ sự phát triển của não bộ và hệ xương của thai nhi.', N'DM1       ')
INSERT [dbo].[SUA] ([ID], [TieuDe], [AnhBia], [SoLuong], [GiaBan], [Mota], [IDDM]) VALUES (2, N'Optimum Gold', N'sb2.jpg', 120, 235000.0000, N'Bổ sung 25% DHA từ tảo (2), hỗ trợ phát triển não bộ và giúp đáp ứng hàm lượng theo khuyến nghị hằng ngày của các chuyên gia y tế Thế Giới FAO/WHO (3).', N'DM1       ')
INSERT [dbo].[SUA] ([ID], [TieuDe], [AnhBia], [SoLuong], [GiaBan], [Mota], [IDDM]) VALUES (3, N'Dielac Alpha Gold IQ', N'sb3.jpg', 200, 350000.0000, N'Các vi chất Kẽm, Selen, Vitamin A, D3, C giúp tăng cường sức đề kháng, bảo vệ trẻ luôn khoẻ mạnh, chống lại các bệnh nhiểm khuẩn khi tiếp xúc nhiều hơn với môi trường xung quanh.', N'DM1       ')
INSERT [dbo].[SUA] ([ID], [TieuDe], [AnhBia], [SoLuong], [GiaBan], [Mota], [IDDM]) VALUES (4, N'Dielac Grow Plus', N'', 2503, 350000.0000, N'Đạm Whey giàu Alpha-Lactalbumin cung cấp axít amin thiết yếu cùng Lysin, chất béo hỗ trợ tăng khả năng hấp thu, giúp trẻ tăng cân khỏe mạnh.Kẽm cùng vitamin nhóm B thúc đẩy quá trình chuyển hóa năng lượng, giúp trẻ ăn ngon miệng.', N'DM1       ')
INSERT [dbo].[SUA] ([ID], [TieuDe], [AnhBia], [SoLuong], [GiaBan], [Mota], [IDDM]) VALUES (5, N'Sữa đặc vinamilk tài lộc', N'sd1.jpg', 120, 75000.0000, N'Creamer đặc có đường Vinamilk Tài Lộc:
- Công thức độc đáo, thơm béo ngọt dịu.
- Đặc chế cho các món sinh tố, trái cây dầm, rau cau, chè, cà phê… giúp tăng hương vị thơm ngon khi chế biến.', N'DM2       ')
INSERT [dbo].[SUA] ([ID], [TieuDe], [AnhBia], [SoLuong], [GiaBan], [Mota], [IDDM]) VALUES (6, N'Sữa đặc ngôi sao phương nam', N'sd2.jpg', 125, 80000.0000, N'Hương nâu nóng nồng nàn Hà Nội, chất hào sảng ly phin
Sài Gòn hay cốc bạc xỉu đậm đà sẻ chia... tất cả được
hòa quyện cùng vị cà phê đắng dịu và hương creamer đặc
Ngôi Sao Phương Nam ngọt ngào, mang đến cho bạn những
khoảnh khắc thưởng thức tuyệt vời nhất.', N'DM2       ')
INSERT [dbo].[SUA] ([ID], [TieuDe], [AnhBia], [SoLuong], [GiaBan], [Mota], [IDDM]) VALUES (7, N'Sữa đặc ông thọ', N'sd3.jpg', 150, 60000.0000, N'Vị ngon cùng năm tháng', N'DM2       ')
INSERT [dbo].[SUA] ([ID], [TieuDe], [AnhBia], [SoLuong], [GiaBan], [Mota], [IDDM]) VALUES (8, N'Sữa đặc quánh', N'sd4.jpg', 5, 10000.0000, N'Đặc quánh', N'DM2       ')
INSERT [dbo].[SUA] ([ID], [TieuDe], [AnhBia], [SoLuong], [GiaBan], [Mota], [IDDM]) VALUES (9, N'Sữa đậu nành tươi', N'sdn1.jpg', 1000, 8000.0000, N'Sữa đậu nành TƯƠI Vinamilk là sự kết hợp độc đáo từ hạt đậu nành không biến đổi gen & dòng Sữa tươi giàu dinh dưỡng, gấp đôi Canxi, giúp xương chắc khỏe, cho mẹ thêm dẻo dai tươi tắn cả ngày.', N'DM3       ')
INSERT [dbo].[SUA] ([ID], [TieuDe], [AnhBia], [SoLuong], [GiaBan], [Mota], [IDDM]) VALUES (10, N'Sữa đậu nành đậu đỏ', N'sdn2.jpg', 800, 7000.0000, N'Sữa đậu nành Đậu đỏ Vinamilk là sự kết hợp hoàn hảo giữa đậu đỏ ngọt thanh, mát lành cùng đậu nành thơm béo. Không chỉ giảm 26% lượng đường mà còn bổ sung vitamin A, D3, E, PP và vitamin nhóm B, mang lại lợi ích 3 TỐT cho cả gia đình.', N'DM3       ')
INSERT [dbo].[SUA] ([ID], [TieuDe], [AnhBia], [SoLuong], [GiaBan], [Mota], [IDDM]) VALUES (11, N'Sữa đậu nành hạnh nhân', N'sdn3.jpg', 800, 7000.0000, N'Sữa đậu nành Hạnh nhân Vinamilk là sự kết hợp hoàn hảo giữa hạnh nhân thơm béo đậm đà cùng đậu nành thanh mát. Không chỉ giảm 44% lượng đường mà còn bổ sung vitamin A, D3, E, PP và Omega 3, mang lại lợi ích 3 TỐT cho cả gia đình.', N'DM3       ')
INSERT [dbo].[SUA] ([ID], [TieuDe], [AnhBia], [SoLuong], [GiaBan], [Mota], [IDDM]) VALUES (12, N'Sữa đậu nành hạt hóc chó', N'sdn4.jpg', 10000, 10000.0000, N'Sữa đậu nành Hạt óc chó Vinamilk là sự kết hợp hoàn hảo giữa hạt óc chó thơm béo đậm đà cùng đậu nành thanh mát. Không chỉ giảm 42% lượng đường mà còn bổ sung vitamin A, D3, E, PP và Omega 3, mang lại lợi ích 3 TỐT cho cả gia đình.', N'DM3       ')
INSERT [dbo].[SUA] ([ID], [TieuDe], [AnhBia], [SoLuong], [GiaBan], [Mota], [IDDM]) VALUES (13, N'Sữa tươi Vinamilk 100% Organic', N'sn1.jpg', 10000, 13000.0000, N'Tại trang trại Vinamilk Organic chuẩn Châu Âu trên cao nguyên Đà Lạt, đàn bò Organic thuần chủng được tận hưởng không khí mát mẻ trong lành, thưởng thứcnhững luống cỏ Organic không thuốc trừ sâu. Mang đến nguồn sữa tươi cao cấp Vinamilk 100% Organic - giữ trọn vẹn những gì tươi ngon thuần khiết nhất đến từ thiên nhiên để gia đình cùng tận hưởng mỗi ngày', N'DM4       ')
INSERT [dbo].[SUA] ([ID], [TieuDe], [AnhBia], [SoLuong], [GiaBan], [Mota], [IDDM]) VALUES (14, N'Sữa tươi tiệt trùng', N'sn2.jpg', 7000, 8000.0000, N'Sữa tươi Vinamilk chứa tổ yến sạch tinh chế hòa quyện cùng
nguồn sữa thuần khiết là món quà sức khỏe thượng hạng cho cả gia đình.', N'DM4       ')
INSERT [dbo].[SUA] ([ID], [TieuDe], [AnhBia], [SoLuong], [GiaBan], [Mota], [IDDM]) VALUES (15, N'Sữa tươi vinamilk green farm', N'sn3.jpg', 10000, 12000.0000, N'Sữa tươi tiệt trùng ít đường', N'DM4       ')
INSERT [dbo].[SUA] ([ID], [TieuDe], [AnhBia], [SoLuong], [GiaBan], [Mota], [IDDM]) VALUES (16, N'SuSu', N'sn4.jpg', 10000, 12000.0000, N'Thức uống Cacao lúa mạch Super Susu với Canxi và dưỡng chất từ sữa và lúa mạch,
bổ sung Vitamin nhóm B và Choline cung cấp nguồn năng lượng mạnh mẽ,
giúp con luôn tỉnh táo, hào hứng trong học tập; nổi bật và thể hiện phong cách thật "đỉnh" trong mỗi cuộc chơi', N'DM4       ')
INSERT [dbo].[SUA] ([ID], [TieuDe], [AnhBia], [SoLuong], [GiaBan], [Mota], [IDDM]) VALUES (17, N'Love yogurt', N'sc1.jpg', 500, 10000.0000, N'
Vị ngon mê hoặc

Tận hưởng hương vị mê hoặc của Sữa chua Vinamilk Love Yogurt với các nguyên liệu cao cấp. Hãy cùng tìm hiểu!', N'DM5       ')
INSERT [dbo].[SUA] ([ID], [TieuDe], [AnhBia], [SoLuong], [GiaBan], [Mota], [IDDM]) VALUES (18, N'Proby', N'sc2.jpg', 300, 8200.0000, N'Tăng sức đề kháng cơ thể

Bổ sung lợi khuẩn Probiotics CHR.HANSEN L.CASEI 431™ có trong sữa chua Vinamilk Probi hàng ngày sẽ giúp hỗ trợ tiêu hóa và tăng sức đề kháng cho gia đình bạn.', N'DM5       ')
INSERT [dbo].[SUA] ([ID], [TieuDe], [AnhBia], [SoLuong], [GiaBan], [Mota], [IDDM]) VALUES (19, N'Hero', N'sc3.jpg', 300, 8300.0000, N'Năng lượng mạnh mẽ,
trẻ làm điều hay

Giàu dưỡng chất từ sữa và nước trái cây ngon tuyệt, cùng với Canxi & Vitamin D3 giúp xương chắc khỏe, Vitamin A cho đôi mắt sáng tinh anh cùng các vitamin nhóm B, giúp trẻ luôn tràn đầy năng lượng và sảng khoái.', N'DM5       ')
INSERT [dbo].[SUA] ([ID], [TieuDe], [AnhBia], [SoLuong], [GiaBan], [Mota], [IDDM]) VALUES (20, N'Yomilk', N'sc4.jpg', 200, 9000.0000, N'Đẹp da đẹp dáng

Sữa chua Vinamilk Nha đam, Lựu đỏ chua chua ngọt ngọt, thêm các hạt nha đam tươi ngon cùng thạch dừa giòn dai giúp thanh mát, nuôi dưỡng làn da xinh đẹp hơn mỗi ngày.', N'DM5       ')
INSERT [dbo].[SUA] ([ID], [TieuDe], [AnhBia], [SoLuong], [GiaBan], [Mota], [IDDM]) VALUES (23, N'100', N'', NULL, NULL, NULL, N'DM1       ')
SET IDENTITY_INSERT [dbo].[SUA] OFF
GO
INSERT [dbo].[TAIKHOAN] ([Ten], [MatKhau], [QuenTC]) VALUES (N'admin     ', N'admin     ', N'admin     ')
INSERT [dbo].[TAIKHOAN] ([Ten], [MatKhau], [QuenTC]) VALUES (N'linh      ', N'28042007  ', N'user      ')
INSERT [dbo].[TAIKHOAN] ([Ten], [MatKhau], [QuenTC]) VALUES (N'phong     ', N'23102000  ', N'user      ')
GO
ALTER TABLE [dbo].[SUA]  WITH CHECK ADD  CONSTRAINT [FK_SUA_DMSUA] FOREIGN KEY([IDDM])
REFERENCES [dbo].[DMSUA] ([IDDM])
GO
ALTER TABLE [dbo].[SUA] CHECK CONSTRAINT [FK_SUA_DMSUA]
GO
USE [master]
GO
ALTER DATABASE [VINAMILK] SET  READ_WRITE 
GO
