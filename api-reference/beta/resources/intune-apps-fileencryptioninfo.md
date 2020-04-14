---
title: Тип ресурса fileEncryptionInfo
description: Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0e5eaa2e993fb56eeb56b7e147963a0b8df03cae
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459099"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="b7540-103">Тип ресурса fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="b7540-103">fileEncryptionInfo resource type</span></span>

<span data-ttu-id="b7540-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b7540-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b7540-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b7540-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7540-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b7540-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7540-107">Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="b7540-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="b7540-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b7540-108">Properties</span></span>
|<span data-ttu-id="b7540-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b7540-109">Property</span></span>|<span data-ttu-id="b7540-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b7540-110">Type</span></span>|<span data-ttu-id="b7540-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b7540-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7540-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="b7540-112">encryptionKey</span></span>|<span data-ttu-id="b7540-113">Binary</span><span class="sxs-lookup"><span data-stu-id="b7540-113">Binary</span></span>|<span data-ttu-id="b7540-114">Ключ, используемый для шифрования содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="b7540-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="b7540-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="b7540-115">initializationVector</span></span>|<span data-ttu-id="b7540-116">Binary</span><span class="sxs-lookup"><span data-stu-id="b7540-116">Binary</span></span>|<span data-ttu-id="b7540-117">Вектор инициализации, используемый для алгоритма шифрования.</span><span class="sxs-lookup"><span data-stu-id="b7540-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="b7540-118">mac</span><span class="sxs-lookup"><span data-stu-id="b7540-118">mac</span></span>|<span data-ttu-id="b7540-119">Binary</span><span class="sxs-lookup"><span data-stu-id="b7540-119">Binary</span></span>|<span data-ttu-id="b7540-120">Хэш зашифрованного содержимого файла + IV (хэш содержимого).</span><span class="sxs-lookup"><span data-stu-id="b7540-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="b7540-121">macKey</span><span class="sxs-lookup"><span data-stu-id="b7540-121">macKey</span></span>|<span data-ttu-id="b7540-122">Binary</span><span class="sxs-lookup"><span data-stu-id="b7540-122">Binary</span></span>|<span data-ttu-id="b7540-123">Ключ для получения свойства mac.</span><span class="sxs-lookup"><span data-stu-id="b7540-123">The key used to get mac.</span></span>|
|<span data-ttu-id="b7540-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="b7540-124">profileIdentifier</span></span>|<span data-ttu-id="b7540-125">String</span><span class="sxs-lookup"><span data-stu-id="b7540-125">String</span></span>|<span data-ttu-id="b7540-126">Идентификатор профиля.</span><span class="sxs-lookup"><span data-stu-id="b7540-126">The the profile identifier.</span></span>|
|<span data-ttu-id="b7540-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="b7540-127">fileDigest</span></span>|<span data-ttu-id="b7540-128">Binary</span><span class="sxs-lookup"><span data-stu-id="b7540-128">Binary</span></span>|<span data-ttu-id="b7540-129">Дайджест файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="b7540-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="b7540-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="b7540-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="b7540-131">String</span><span class="sxs-lookup"><span data-stu-id="b7540-131">String</span></span>|<span data-ttu-id="b7540-132">Алгоритм дайджеста файла.</span><span class="sxs-lookup"><span data-stu-id="b7540-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7540-133">Отношения</span><span class="sxs-lookup"><span data-stu-id="b7540-133">Relationships</span></span>
<span data-ttu-id="b7540-134">Нет</span><span class="sxs-lookup"><span data-stu-id="b7540-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7540-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b7540-135">JSON Representation</span></span>
<span data-ttu-id="b7540-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b7540-136">Here is a JSON representation of the resource.</span></span>
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



