---
title: Тип ресурса fileEncryptionInfo
description: Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3c5586b3107e8b7039df7068d0ab6b00e81bf4b5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42798135"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="b3b68-103">Тип ресурса fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="b3b68-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="b3b68-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b3b68-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3b68-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b3b68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3b68-106">Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="b3b68-106">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="b3b68-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="b3b68-107">Properties</span></span>
|<span data-ttu-id="b3b68-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3b68-108">Property</span></span>|<span data-ttu-id="b3b68-109">Тип</span><span class="sxs-lookup"><span data-stu-id="b3b68-109">Type</span></span>|<span data-ttu-id="b3b68-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b3b68-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3b68-111">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="b3b68-111">encryptionKey</span></span>|<span data-ttu-id="b3b68-112">Binary</span><span class="sxs-lookup"><span data-stu-id="b3b68-112">Binary</span></span>|<span data-ttu-id="b3b68-113">Ключ, используемый для шифрования содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="b3b68-113">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="b3b68-114">initializationVector</span><span class="sxs-lookup"><span data-stu-id="b3b68-114">initializationVector</span></span>|<span data-ttu-id="b3b68-115">Binary</span><span class="sxs-lookup"><span data-stu-id="b3b68-115">Binary</span></span>|<span data-ttu-id="b3b68-116">Вектор инициализации, используемый для алгоритма шифрования.</span><span class="sxs-lookup"><span data-stu-id="b3b68-116">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="b3b68-117">mac</span><span class="sxs-lookup"><span data-stu-id="b3b68-117">mac</span></span>|<span data-ttu-id="b3b68-118">Binary</span><span class="sxs-lookup"><span data-stu-id="b3b68-118">Binary</span></span>|<span data-ttu-id="b3b68-119">Хэш зашифрованного содержимого файла + IV (хэш содержимого).</span><span class="sxs-lookup"><span data-stu-id="b3b68-119">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="b3b68-120">macKey</span><span class="sxs-lookup"><span data-stu-id="b3b68-120">macKey</span></span>|<span data-ttu-id="b3b68-121">Binary</span><span class="sxs-lookup"><span data-stu-id="b3b68-121">Binary</span></span>|<span data-ttu-id="b3b68-122">Ключ для получения свойства mac.</span><span class="sxs-lookup"><span data-stu-id="b3b68-122">The key used to get mac.</span></span>|
|<span data-ttu-id="b3b68-123">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="b3b68-123">profileIdentifier</span></span>|<span data-ttu-id="b3b68-124">String</span><span class="sxs-lookup"><span data-stu-id="b3b68-124">String</span></span>|<span data-ttu-id="b3b68-125">Идентификатор профиля.</span><span class="sxs-lookup"><span data-stu-id="b3b68-125">The the profile identifier.</span></span>|
|<span data-ttu-id="b3b68-126">fileDigest</span><span class="sxs-lookup"><span data-stu-id="b3b68-126">fileDigest</span></span>|<span data-ttu-id="b3b68-127">Binary</span><span class="sxs-lookup"><span data-stu-id="b3b68-127">Binary</span></span>|<span data-ttu-id="b3b68-128">Дайджест файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="b3b68-128">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="b3b68-129">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="b3b68-129">fileDigestAlgorithm</span></span>|<span data-ttu-id="b3b68-130">String</span><span class="sxs-lookup"><span data-stu-id="b3b68-130">String</span></span>|<span data-ttu-id="b3b68-131">Алгоритм дайджеста файла.</span><span class="sxs-lookup"><span data-stu-id="b3b68-131">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3b68-132">Связи</span><span class="sxs-lookup"><span data-stu-id="b3b68-132">Relationships</span></span>
<span data-ttu-id="b3b68-133">Нет</span><span class="sxs-lookup"><span data-stu-id="b3b68-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3b68-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b3b68-134">JSON Representation</span></span>
<span data-ttu-id="b3b68-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b3b68-135">Here is a JSON representation of the resource.</span></span>
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



