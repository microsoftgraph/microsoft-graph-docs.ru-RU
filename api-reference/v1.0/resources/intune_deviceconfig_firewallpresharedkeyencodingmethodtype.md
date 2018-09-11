# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="00f1a-101">тип перечисления firewallPreSharedKeyEncodingMethodType</span><span class="sxs-lookup"><span data-stu-id="00f1a-101">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="00f1a-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="00f1a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00f1a-103">Возможные значения для firewallPreSharedKeyEncodingMethod</span><span class="sxs-lookup"><span data-stu-id="00f1a-103">Possible values for firewallPreSharedKeyEncodingMethod</span></span>
## <a name="members"></a><span data-ttu-id="00f1a-104">Члены</span><span class="sxs-lookup"><span data-stu-id="00f1a-104">Members</span></span>
|<span data-ttu-id="00f1a-105">Член</span><span class="sxs-lookup"><span data-stu-id="00f1a-105">Member</span></span>|<span data-ttu-id="00f1a-106">Значение</span><span class="sxs-lookup"><span data-stu-id="00f1a-106">Value</span></span>|<span data-ttu-id="00f1a-107">Описание</span><span class="sxs-lookup"><span data-stu-id="00f1a-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00f1a-108">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="00f1a-108">deviceDefault</span></span>|<span data-ttu-id="00f1a-109">0</span><span class="sxs-lookup"><span data-stu-id="00f1a-109">0%</span></span>|<span data-ttu-id="00f1a-110">Intune не настраивает какое-либо значение, не переопределять значение устройства, установленное пользователем по умолчанию</span><span class="sxs-lookup"><span data-stu-id="00f1a-110">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="00f1a-111">none</span><span class="sxs-lookup"><span data-stu-id="00f1a-111">none</span></span>|<span data-ttu-id="00f1a-112">1</span><span class="sxs-lookup"><span data-stu-id="00f1a-112">-1</span></span>|<span data-ttu-id="00f1a-113">Предварительный ключ не кодируется.</span><span class="sxs-lookup"><span data-stu-id="00f1a-113">Preshared key is not encoded.</span></span> <span data-ttu-id="00f1a-114">Вместо этого он будет храниться в формате расширенных символов</span><span class="sxs-lookup"><span data-stu-id="00f1a-114">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="00f1a-115">utF8</span><span class="sxs-lookup"><span data-stu-id="00f1a-115">utf-8</span></span>|<span data-ttu-id="00f1a-116">2</span><span class="sxs-lookup"><span data-stu-id="00f1a-116">2</span></span>|<span data-ttu-id="00f1a-117">Кодирование предварительного ключа с помощью UTF-8</span><span class="sxs-lookup"><span data-stu-id="00f1a-117">Encode the preshared key using UTF-8</span></span>|








