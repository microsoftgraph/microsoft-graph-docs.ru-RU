# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="27bcf-101">Тип ресурса fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="27bcf-101">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="27bcf-102">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="27bcf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27bcf-103">Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="27bcf-103">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="27bcf-104">Свойства</span><span class="sxs-lookup"><span data-stu-id="27bcf-104">Properties</span></span>
|<span data-ttu-id="27bcf-105">Свойство</span><span class="sxs-lookup"><span data-stu-id="27bcf-105">Property</span></span>|<span data-ttu-id="27bcf-106">Тип</span><span class="sxs-lookup"><span data-stu-id="27bcf-106">Type</span></span>|<span data-ttu-id="27bcf-107">Описание</span><span class="sxs-lookup"><span data-stu-id="27bcf-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27bcf-108">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="27bcf-108">encryptionKey</span></span>|<span data-ttu-id="27bcf-109">Binary</span><span class="sxs-lookup"><span data-stu-id="27bcf-109">Binary</span></span>|<span data-ttu-id="27bcf-110">Ключ, используемый для шифрования содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="27bcf-110">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="27bcf-111">initializationVector</span><span class="sxs-lookup"><span data-stu-id="27bcf-111">initializationVector</span></span>|<span data-ttu-id="27bcf-112">Binary</span><span class="sxs-lookup"><span data-stu-id="27bcf-112">Binary</span></span>|<span data-ttu-id="27bcf-113">Вектор инициализации, используемый для алгоритма шифрования.</span><span class="sxs-lookup"><span data-stu-id="27bcf-113">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="27bcf-114">mac</span><span class="sxs-lookup"><span data-stu-id="27bcf-114">mac</span></span>|<span data-ttu-id="27bcf-115">Binary</span><span class="sxs-lookup"><span data-stu-id="27bcf-115">Binary</span></span>|<span data-ttu-id="27bcf-116">Хэш зашифрованного содержимого файла + IV (хэш содержимого).</span><span class="sxs-lookup"><span data-stu-id="27bcf-116">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="27bcf-117">macKey</span><span class="sxs-lookup"><span data-stu-id="27bcf-117">macKey</span></span>|<span data-ttu-id="27bcf-118">Binary</span><span class="sxs-lookup"><span data-stu-id="27bcf-118">Binary</span></span>|<span data-ttu-id="27bcf-119">Ключ для получения свойства mac.</span><span class="sxs-lookup"><span data-stu-id="27bcf-119">The key used to get mac.</span></span>|
|<span data-ttu-id="27bcf-120">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="27bcf-120">profileIdentifier</span></span>|<span data-ttu-id="27bcf-121">String</span><span class="sxs-lookup"><span data-stu-id="27bcf-121">String</span></span>|<span data-ttu-id="27bcf-122">Идентификатор профиля.</span><span class="sxs-lookup"><span data-stu-id="27bcf-122">The the profile identifier.</span></span>|
|<span data-ttu-id="27bcf-123">fileDigest</span><span class="sxs-lookup"><span data-stu-id="27bcf-123">fileDigest</span></span>|<span data-ttu-id="27bcf-124">Binary</span><span class="sxs-lookup"><span data-stu-id="27bcf-124">Binary</span></span>|<span data-ttu-id="27bcf-125">Дайджест файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="27bcf-125">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="27bcf-126">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="27bcf-126">fileDigestAlgorithm</span></span>|<span data-ttu-id="27bcf-127">String</span><span class="sxs-lookup"><span data-stu-id="27bcf-127">String</span></span>|<span data-ttu-id="27bcf-128">Алгоритм дайджеста файла.</span><span class="sxs-lookup"><span data-stu-id="27bcf-128">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="27bcf-129">Связи</span><span class="sxs-lookup"><span data-stu-id="27bcf-129">Relationships</span></span>
<span data-ttu-id="27bcf-130">Нет</span><span class="sxs-lookup"><span data-stu-id="27bcf-130">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="27bcf-131">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="27bcf-131">JSON Representation</span></span>
<span data-ttu-id="27bcf-132">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="27bcf-132">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.fileEncryptionInfo"
}-->
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








