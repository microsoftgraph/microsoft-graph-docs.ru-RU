# <a name="firewallcertificaterevocationlistcheckmethodtype-enum-type"></a><span data-ttu-id="1d68d-101">Тип перечисления firewallCertificateRevocationListCheckMethodType</span><span class="sxs-lookup"><span data-stu-id="1d68d-101">firewallCertificateRevocationListCheckMethodType enum type</span></span>

> <span data-ttu-id="1d68d-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="1d68d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1d68d-103">Возможные значения для firewallCertificateRevocationListCheckMethod</span><span class="sxs-lookup"><span data-stu-id="1d68d-103">Possible values for firewallCertificateRevocationListCheckMethod</span></span>
## <a name="members"></a><span data-ttu-id="1d68d-104">Элементы</span><span class="sxs-lookup"><span data-stu-id="1d68d-104">Members</span></span>
|<span data-ttu-id="1d68d-105">Элемент</span><span class="sxs-lookup"><span data-stu-id="1d68d-105">Member</span></span>|<span data-ttu-id="1d68d-106">Значение</span><span class="sxs-lookup"><span data-stu-id="1d68d-106">Value</span></span>|<span data-ttu-id="1d68d-107">Описание</span><span class="sxs-lookup"><span data-stu-id="1d68d-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d68d-108">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="1d68d-108">deviceDefault</span></span>|<span data-ttu-id="1d68d-109">0</span><span class="sxs-lookup"><span data-stu-id="1d68d-109">0%</span></span>|<span data-ttu-id="1d68d-110">Intune не настраивает какое-либо значение, не переопределять значение устройства, установленное пользователем по умолчанию</span><span class="sxs-lookup"><span data-stu-id="1d68d-110">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="1d68d-111">none</span><span class="sxs-lookup"><span data-stu-id="1d68d-111">none</span></span>|<span data-ttu-id="1d68d-112">1</span><span class="sxs-lookup"><span data-stu-id="1d68d-112">-1</span></span>|<span data-ttu-id="1d68d-113">Не проверять список отзывов сертификатов</span><span class="sxs-lookup"><span data-stu-id="1d68d-113">Do not check certificate revocation list</span></span>|
|<span data-ttu-id="1d68d-114">попытаться</span><span class="sxs-lookup"><span data-stu-id="1d68d-114">attempt</span></span>|<span data-ttu-id="1d68d-115">2</span><span class="sxs-lookup"><span data-stu-id="1d68d-115">2</span></span>|<span data-ttu-id="1d68d-116">Попытаться проверить список отзывов сертификатов и разрешить сертификат только в случае, если сертификат подтверждается при проверке</span><span class="sxs-lookup"><span data-stu-id="1d68d-116">Attempt CRL check and allow a certificate only if the certificate is confirmed by the check</span></span>|
|<span data-ttu-id="1d68d-117">require</span><span class="sxs-lookup"><span data-stu-id="1d68d-117">Require</span></span>|<span data-ttu-id="1d68d-118">3</span><span class="sxs-lookup"><span data-stu-id="1d68d-118">3</span></span>|<span data-ttu-id="1d68d-119">Требовать успешной проверки списка отзывов сертификатов перед разрешением сертификата</span><span class="sxs-lookup"><span data-stu-id="1d68d-119">Require a successful CRL check before allowing a certificate</span></span>|








