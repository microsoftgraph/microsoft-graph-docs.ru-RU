# <a name="managedappclipboardsharinglevel-enum-type"></a><span data-ttu-id="76af7-101">тип перечисления managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="76af7-101">managedAppClipboardSharingLevel enum type</span></span>

> <span data-ttu-id="76af7-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="76af7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="76af7-103">Указывает на уровень общего доступа приложений к буферу обмена на устройстве</span><span class="sxs-lookup"><span data-stu-id="76af7-103">The level to which the clipboard may be shared between apps on the managed device.</span></span>
## <a name="members"></a><span data-ttu-id="76af7-104">Элементы</span><span class="sxs-lookup"><span data-stu-id="76af7-104">Members</span></span>
|<span data-ttu-id="76af7-105">Элемент</span><span class="sxs-lookup"><span data-stu-id="76af7-105">Member</span></span>|<span data-ttu-id="76af7-106">Значение</span><span class="sxs-lookup"><span data-stu-id="76af7-106">Value</span></span>|<span data-ttu-id="76af7-107">Описание</span><span class="sxs-lookup"><span data-stu-id="76af7-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76af7-108">allApps</span><span class="sxs-lookup"><span data-stu-id="76af7-108">allApps</span></span>|<span data-ttu-id="76af7-109">0</span><span class="sxs-lookup"><span data-stu-id="76af7-109">0%</span></span>|<span data-ttu-id="76af7-110">Общий доступ разрешен между всеми приложениями, управляемыми или нет</span><span class="sxs-lookup"><span data-stu-id="76af7-110">Sharing is allowed between all apps, managed or not</span></span>|
|<span data-ttu-id="76af7-111">managedAppsWithPasteIn</span><span class="sxs-lookup"><span data-stu-id="76af7-111">managedAppsWithPasteIn</span></span>|<span data-ttu-id="76af7-112">1</span><span class="sxs-lookup"><span data-stu-id="76af7-112">-1</span></span>|<span data-ttu-id="76af7-113">Общий доступ разрешен между всеми управляемыми приложениями с помощью включенной вставки</span><span class="sxs-lookup"><span data-stu-id="76af7-113">Sharing is allowed between all managed apps with paste in enabled</span></span>|
|<span data-ttu-id="76af7-114">managedApps</span><span class="sxs-lookup"><span data-stu-id="76af7-114">managedApps</span></span>|<span data-ttu-id="76af7-115">2</span><span class="sxs-lookup"><span data-stu-id="76af7-115">2</span></span>|<span data-ttu-id="76af7-116">Общий доступ разрешен между всеми управляемыми приложениями</span><span class="sxs-lookup"><span data-stu-id="76af7-116">Sharing is allowed between all managed apps</span></span>|
|<span data-ttu-id="76af7-117">заблокировано</span><span class="sxs-lookup"><span data-stu-id="76af7-117">blocked</span></span>|<span data-ttu-id="76af7-118">3</span><span class="sxs-lookup"><span data-stu-id="76af7-118">3</span></span>|<span data-ttu-id="76af7-119">Общий доступ между приложениями отключен</span><span class="sxs-lookup"><span data-stu-id="76af7-119">Sharing between apps is disabled</span></span>|








