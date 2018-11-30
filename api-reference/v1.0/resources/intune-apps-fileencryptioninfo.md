---
title: Тип ресурса fileEncryptionInfo
description: Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.
ms.openlocfilehash: 92aceaa56221287dcde67dcefb4d9ae7109d9273
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/29/2018
ms.locfileid: "27027837"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="0278e-103">Тип ресурса fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="0278e-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="0278e-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="0278e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0278e-105">Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="0278e-105">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="0278e-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="0278e-106">Properties</span></span>
|<span data-ttu-id="0278e-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="0278e-107">Property</span></span>|<span data-ttu-id="0278e-108">Тип</span><span class="sxs-lookup"><span data-stu-id="0278e-108">Type</span></span>|<span data-ttu-id="0278e-109">Описание</span><span class="sxs-lookup"><span data-stu-id="0278e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0278e-110">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="0278e-110">encryptionKey</span></span>|<span data-ttu-id="0278e-111">Binary</span><span class="sxs-lookup"><span data-stu-id="0278e-111">Binary</span></span>|<span data-ttu-id="0278e-112">Ключ, используемый для шифрования содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="0278e-112">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="0278e-113">initializationVector</span><span class="sxs-lookup"><span data-stu-id="0278e-113">initializationVector</span></span>|<span data-ttu-id="0278e-114">Binary</span><span class="sxs-lookup"><span data-stu-id="0278e-114">Binary</span></span>|<span data-ttu-id="0278e-115">Вектор инициализации, используемый для алгоритма шифрования.</span><span class="sxs-lookup"><span data-stu-id="0278e-115">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="0278e-116">mac</span><span class="sxs-lookup"><span data-stu-id="0278e-116">mac</span></span>|<span data-ttu-id="0278e-117">Binary</span><span class="sxs-lookup"><span data-stu-id="0278e-117">Binary</span></span>|<span data-ttu-id="0278e-118">Хэш зашифрованного содержимого файла + IV (хэш содержимого).</span><span class="sxs-lookup"><span data-stu-id="0278e-118">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="0278e-119">macKey</span><span class="sxs-lookup"><span data-stu-id="0278e-119">macKey</span></span>|<span data-ttu-id="0278e-120">Binary</span><span class="sxs-lookup"><span data-stu-id="0278e-120">Binary</span></span>|<span data-ttu-id="0278e-121">Ключ для получения свойства mac.</span><span class="sxs-lookup"><span data-stu-id="0278e-121">The key used to get mac.</span></span>|
|<span data-ttu-id="0278e-122">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="0278e-122">profileIdentifier</span></span>|<span data-ttu-id="0278e-123">String</span><span class="sxs-lookup"><span data-stu-id="0278e-123">String</span></span>|<span data-ttu-id="0278e-124">Идентификатор профиля.</span><span class="sxs-lookup"><span data-stu-id="0278e-124">The the profile identifier.</span></span>|
|<span data-ttu-id="0278e-125">fileDigest</span><span class="sxs-lookup"><span data-stu-id="0278e-125">fileDigest</span></span>|<span data-ttu-id="0278e-126">Binary</span><span class="sxs-lookup"><span data-stu-id="0278e-126">Binary</span></span>|<span data-ttu-id="0278e-127">Дайджест файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="0278e-127">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="0278e-128">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="0278e-128">fileDigestAlgorithm</span></span>|<span data-ttu-id="0278e-129">String</span><span class="sxs-lookup"><span data-stu-id="0278e-129">String</span></span>|<span data-ttu-id="0278e-130">Алгоритм дайджеста файла.</span><span class="sxs-lookup"><span data-stu-id="0278e-130">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0278e-131">Связи</span><span class="sxs-lookup"><span data-stu-id="0278e-131">Relationships</span></span>
<span data-ttu-id="0278e-132">Нет</span><span class="sxs-lookup"><span data-stu-id="0278e-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0278e-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="0278e-133">JSON Representation</span></span>
<span data-ttu-id="0278e-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="0278e-134">Here is a JSON representation of the resource.</span></span>
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



