---
title: Тип ресурса fileEncryptionInfo
description: Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e0dff917b9fc6dc8bc99cb388cdf0f461dc394c3
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356291"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="f2a51-103">Тип ресурса fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="f2a51-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="f2a51-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f2a51-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2a51-105">Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="f2a51-105">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="f2a51-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="f2a51-106">Properties</span></span>
|<span data-ttu-id="f2a51-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="f2a51-107">Property</span></span>|<span data-ttu-id="f2a51-108">Тип</span><span class="sxs-lookup"><span data-stu-id="f2a51-108">Type</span></span>|<span data-ttu-id="f2a51-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f2a51-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2a51-110">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="f2a51-110">encryptionKey</span></span>|<span data-ttu-id="f2a51-111">Binary</span><span class="sxs-lookup"><span data-stu-id="f2a51-111">Binary</span></span>|<span data-ttu-id="f2a51-112">Ключ, используемый для шифрования содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="f2a51-112">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="f2a51-113">initializationVector</span><span class="sxs-lookup"><span data-stu-id="f2a51-113">initializationVector</span></span>|<span data-ttu-id="f2a51-114">Binary</span><span class="sxs-lookup"><span data-stu-id="f2a51-114">Binary</span></span>|<span data-ttu-id="f2a51-115">Вектор инициализации, используемый для алгоритма шифрования.</span><span class="sxs-lookup"><span data-stu-id="f2a51-115">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="f2a51-116">mac</span><span class="sxs-lookup"><span data-stu-id="f2a51-116">mac</span></span>|<span data-ttu-id="f2a51-117">Binary</span><span class="sxs-lookup"><span data-stu-id="f2a51-117">Binary</span></span>|<span data-ttu-id="f2a51-118">Хэш зашифрованного содержимого файла + IV (хэш содержимого).</span><span class="sxs-lookup"><span data-stu-id="f2a51-118">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="f2a51-119">macKey</span><span class="sxs-lookup"><span data-stu-id="f2a51-119">macKey</span></span>|<span data-ttu-id="f2a51-120">Binary</span><span class="sxs-lookup"><span data-stu-id="f2a51-120">Binary</span></span>|<span data-ttu-id="f2a51-121">Ключ для получения свойства mac.</span><span class="sxs-lookup"><span data-stu-id="f2a51-121">The key used to get mac.</span></span>|
|<span data-ttu-id="f2a51-122">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="f2a51-122">profileIdentifier</span></span>|<span data-ttu-id="f2a51-123">String</span><span class="sxs-lookup"><span data-stu-id="f2a51-123">String</span></span>|<span data-ttu-id="f2a51-124">Идентификатор профиля.</span><span class="sxs-lookup"><span data-stu-id="f2a51-124">The profile identifier.</span></span>|
|<span data-ttu-id="f2a51-125">fileDigest</span><span class="sxs-lookup"><span data-stu-id="f2a51-125">fileDigest</span></span>|<span data-ttu-id="f2a51-126">Binary</span><span class="sxs-lookup"><span data-stu-id="f2a51-126">Binary</span></span>|<span data-ttu-id="f2a51-127">Дайджест файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="f2a51-127">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="f2a51-128">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="f2a51-128">fileDigestAlgorithm</span></span>|<span data-ttu-id="f2a51-129">String</span><span class="sxs-lookup"><span data-stu-id="f2a51-129">String</span></span>|<span data-ttu-id="f2a51-130">Алгоритм дайджеста файла.</span><span class="sxs-lookup"><span data-stu-id="f2a51-130">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2a51-131">Связи</span><span class="sxs-lookup"><span data-stu-id="f2a51-131">Relationships</span></span>
<span data-ttu-id="f2a51-132">Нет</span><span class="sxs-lookup"><span data-stu-id="f2a51-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2a51-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="f2a51-133">JSON Representation</span></span>
<span data-ttu-id="f2a51-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="f2a51-134">Here is a JSON representation of the resource.</span></span>
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




