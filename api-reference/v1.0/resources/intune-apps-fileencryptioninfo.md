---
title: Тип ресурса fileEncryptionInfo
description: Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 66c4fc3c724eecf3a05dae24cb3f6a52de82d059
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255852"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="f952f-103">Тип ресурса fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="f952f-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="f952f-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f952f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f952f-105">Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="f952f-105">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="f952f-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f952f-106">Properties</span></span>
|<span data-ttu-id="f952f-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f952f-107">Property</span></span>|<span data-ttu-id="f952f-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f952f-108">Type</span></span>|<span data-ttu-id="f952f-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f952f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f952f-110">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="f952f-110">encryptionKey</span></span>|<span data-ttu-id="f952f-111">Binary</span><span class="sxs-lookup"><span data-stu-id="f952f-111">Binary</span></span>|<span data-ttu-id="f952f-112">Ключ, используемый для шифрования содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="f952f-112">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="f952f-113">initializationVector</span><span class="sxs-lookup"><span data-stu-id="f952f-113">initializationVector</span></span>|<span data-ttu-id="f952f-114">Binary</span><span class="sxs-lookup"><span data-stu-id="f952f-114">Binary</span></span>|<span data-ttu-id="f952f-115">Вектор инициализации, используемый для алгоритма шифрования.</span><span class="sxs-lookup"><span data-stu-id="f952f-115">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="f952f-116">mac</span><span class="sxs-lookup"><span data-stu-id="f952f-116">mac</span></span>|<span data-ttu-id="f952f-117">Binary</span><span class="sxs-lookup"><span data-stu-id="f952f-117">Binary</span></span>|<span data-ttu-id="f952f-118">Хэш зашифрованного содержимого файла + IV (хэш содержимого).</span><span class="sxs-lookup"><span data-stu-id="f952f-118">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="f952f-119">macKey</span><span class="sxs-lookup"><span data-stu-id="f952f-119">macKey</span></span>|<span data-ttu-id="f952f-120">Binary</span><span class="sxs-lookup"><span data-stu-id="f952f-120">Binary</span></span>|<span data-ttu-id="f952f-121">Ключ для получения свойства mac.</span><span class="sxs-lookup"><span data-stu-id="f952f-121">The key used to get mac.</span></span>|
|<span data-ttu-id="f952f-122">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="f952f-122">profileIdentifier</span></span>|<span data-ttu-id="f952f-123">String</span><span class="sxs-lookup"><span data-stu-id="f952f-123">String</span></span>|<span data-ttu-id="f952f-124">Идентификатор профиля.</span><span class="sxs-lookup"><span data-stu-id="f952f-124">The the profile identifier.</span></span>|
|<span data-ttu-id="f952f-125">fileDigest</span><span class="sxs-lookup"><span data-stu-id="f952f-125">fileDigest</span></span>|<span data-ttu-id="f952f-126">Binary</span><span class="sxs-lookup"><span data-stu-id="f952f-126">Binary</span></span>|<span data-ttu-id="f952f-127">Дайджест файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="f952f-127">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="f952f-128">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="f952f-128">fileDigestAlgorithm</span></span>|<span data-ttu-id="f952f-129">String</span><span class="sxs-lookup"><span data-stu-id="f952f-129">String</span></span>|<span data-ttu-id="f952f-130">Алгоритм дайджеста файла.</span><span class="sxs-lookup"><span data-stu-id="f952f-130">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f952f-131">Связи</span><span class="sxs-lookup"><span data-stu-id="f952f-131">Relationships</span></span>
<span data-ttu-id="f952f-132">Нет</span><span class="sxs-lookup"><span data-stu-id="f952f-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f952f-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f952f-133">JSON Representation</span></span>
<span data-ttu-id="f952f-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f952f-134">Here is a JSON representation of the resource.</span></span>
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



