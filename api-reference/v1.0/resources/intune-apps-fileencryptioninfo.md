---
title: Тип ресурса fileEncryptionInfo
description: Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5f9d9dce2516c1978058dd1c9ddbf2211a3d88da
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620257"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="867c9-103">Тип ресурса fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="867c9-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="867c9-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="867c9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="867c9-105">Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="867c9-105">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="867c9-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="867c9-106">Properties</span></span>
|<span data-ttu-id="867c9-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="867c9-107">Property</span></span>|<span data-ttu-id="867c9-108">Тип</span><span class="sxs-lookup"><span data-stu-id="867c9-108">Type</span></span>|<span data-ttu-id="867c9-109">Описание</span><span class="sxs-lookup"><span data-stu-id="867c9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="867c9-110">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="867c9-110">encryptionKey</span></span>|<span data-ttu-id="867c9-111">Binary</span><span class="sxs-lookup"><span data-stu-id="867c9-111">Binary</span></span>|<span data-ttu-id="867c9-112">Ключ, используемый для шифрования содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="867c9-112">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="867c9-113">initializationVector</span><span class="sxs-lookup"><span data-stu-id="867c9-113">initializationVector</span></span>|<span data-ttu-id="867c9-114">Binary</span><span class="sxs-lookup"><span data-stu-id="867c9-114">Binary</span></span>|<span data-ttu-id="867c9-115">Вектор инициализации, используемый для алгоритма шифрования.</span><span class="sxs-lookup"><span data-stu-id="867c9-115">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="867c9-116">mac</span><span class="sxs-lookup"><span data-stu-id="867c9-116">mac</span></span>|<span data-ttu-id="867c9-117">Binary</span><span class="sxs-lookup"><span data-stu-id="867c9-117">Binary</span></span>|<span data-ttu-id="867c9-118">Хэш зашифрованного содержимого файла + IV (хэш содержимого).</span><span class="sxs-lookup"><span data-stu-id="867c9-118">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="867c9-119">macKey</span><span class="sxs-lookup"><span data-stu-id="867c9-119">macKey</span></span>|<span data-ttu-id="867c9-120">Binary</span><span class="sxs-lookup"><span data-stu-id="867c9-120">Binary</span></span>|<span data-ttu-id="867c9-121">Ключ для получения свойства mac.</span><span class="sxs-lookup"><span data-stu-id="867c9-121">The key used to get mac.</span></span>|
|<span data-ttu-id="867c9-122">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="867c9-122">profileIdentifier</span></span>|<span data-ttu-id="867c9-123">String</span><span class="sxs-lookup"><span data-stu-id="867c9-123">String</span></span>|<span data-ttu-id="867c9-124">Идентификатор профиля.</span><span class="sxs-lookup"><span data-stu-id="867c9-124">The profile identifier.</span></span>|
|<span data-ttu-id="867c9-125">fileDigest</span><span class="sxs-lookup"><span data-stu-id="867c9-125">fileDigest</span></span>|<span data-ttu-id="867c9-126">Binary</span><span class="sxs-lookup"><span data-stu-id="867c9-126">Binary</span></span>|<span data-ttu-id="867c9-127">Дайджест файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="867c9-127">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="867c9-128">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="867c9-128">fileDigestAlgorithm</span></span>|<span data-ttu-id="867c9-129">String</span><span class="sxs-lookup"><span data-stu-id="867c9-129">String</span></span>|<span data-ttu-id="867c9-130">Алгоритм дайджеста файла.</span><span class="sxs-lookup"><span data-stu-id="867c9-130">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="867c9-131">Отношения</span><span class="sxs-lookup"><span data-stu-id="867c9-131">Relationships</span></span>
<span data-ttu-id="867c9-132">Нет</span><span class="sxs-lookup"><span data-stu-id="867c9-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="867c9-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="867c9-133">JSON Representation</span></span>
<span data-ttu-id="867c9-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="867c9-134">Here is a JSON representation of the resource.</span></span>
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



