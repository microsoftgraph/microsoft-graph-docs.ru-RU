# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="f475e-101">Тип ресурса fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="f475e-101">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="f475e-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="f475e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f475e-103">Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="f475e-103">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="f475e-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="f475e-104">Properties</span></span>
|<span data-ttu-id="f475e-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="f475e-105">Property</span></span>|<span data-ttu-id="f475e-106">Тип</span><span class="sxs-lookup"><span data-stu-id="f475e-106">Type</span></span>|<span data-ttu-id="f475e-107">Описание</span><span class="sxs-lookup"><span data-stu-id="f475e-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f475e-108">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="f475e-108">encryptionKey</span></span>|<span data-ttu-id="f475e-109">Binary</span><span class="sxs-lookup"><span data-stu-id="f475e-109">Binary</span></span>|<span data-ttu-id="f475e-110">Ключ, используемый для шифрования содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="f475e-110">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="f475e-111">initializationVector</span><span class="sxs-lookup"><span data-stu-id="f475e-111">initializationVector</span></span>|<span data-ttu-id="f475e-112">Binary</span><span class="sxs-lookup"><span data-stu-id="f475e-112">Binary</span></span>|<span data-ttu-id="f475e-113">Вектор инициализации, используемый для алгоритма шифрования.</span><span class="sxs-lookup"><span data-stu-id="f475e-113">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="f475e-114">mac</span><span class="sxs-lookup"><span data-stu-id="f475e-114">mac</span></span>|<span data-ttu-id="f475e-115">Binary</span><span class="sxs-lookup"><span data-stu-id="f475e-115">Binary</span></span>|<span data-ttu-id="f475e-116">Хэш зашифрованного содержимого файла + IV (хэш содержимого).</span><span class="sxs-lookup"><span data-stu-id="f475e-116">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="f475e-117">macKey</span><span class="sxs-lookup"><span data-stu-id="f475e-117">macKey</span></span>|<span data-ttu-id="f475e-118">Binary</span><span class="sxs-lookup"><span data-stu-id="f475e-118">Binary</span></span>|<span data-ttu-id="f475e-119">Ключ для получения свойства mac.</span><span class="sxs-lookup"><span data-stu-id="f475e-119">The key used to get mac.</span></span>|
|<span data-ttu-id="f475e-120">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="f475e-120">profileIdentifier</span></span>|<span data-ttu-id="f475e-121">String</span><span class="sxs-lookup"><span data-stu-id="f475e-121">String</span></span>|<span data-ttu-id="f475e-122">Идентификатор профиля.</span><span class="sxs-lookup"><span data-stu-id="f475e-122">The the profile identifier.</span></span>|
|<span data-ttu-id="f475e-123">fileDigest</span><span class="sxs-lookup"><span data-stu-id="f475e-123">fileDigest</span></span>|<span data-ttu-id="f475e-124">Binary</span><span class="sxs-lookup"><span data-stu-id="f475e-124">Binary</span></span>|<span data-ttu-id="f475e-125">Дайджест файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="f475e-125">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="f475e-126">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="f475e-126">fileDigestAlgorithm</span></span>|<span data-ttu-id="f475e-127">String</span><span class="sxs-lookup"><span data-stu-id="f475e-127">String</span></span>|<span data-ttu-id="f475e-128">Алгоритм дайджеста файла.</span><span class="sxs-lookup"><span data-stu-id="f475e-128">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f475e-129">Связи</span><span class="sxs-lookup"><span data-stu-id="f475e-129">Relationships</span></span>
<span data-ttu-id="f475e-130">Нет</span><span class="sxs-lookup"><span data-stu-id="f475e-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f475e-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f475e-131">JSON Representation</span></span>
<span data-ttu-id="f475e-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f475e-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileEncryptionInfo"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fileEncryptionInfo",
  "encryptionKey": "binary",
  "initializationVector": "binary",
  "mac": "binary",
  "macKey": "binary",
  "profileIdentifier": "String",
  "fileDigest": "binary",
  "fileDigestAlgorithm": "String"
}
```



