---
title: Тип ресурса fileEncryptionInfo
description: Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5717936692dde3e92071e0f697fa0204bf7550ee
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42493792"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="15d1c-103">Тип ресурса fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="15d1c-103">fileEncryptionInfo resource type</span></span>

<span data-ttu-id="15d1c-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="15d1c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15d1c-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="15d1c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15d1c-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="15d1c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15d1c-107">Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="15d1c-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="15d1c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="15d1c-108">Properties</span></span>
|<span data-ttu-id="15d1c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="15d1c-109">Property</span></span>|<span data-ttu-id="15d1c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="15d1c-110">Type</span></span>|<span data-ttu-id="15d1c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="15d1c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15d1c-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="15d1c-112">encryptionKey</span></span>|<span data-ttu-id="15d1c-113">Binary</span><span class="sxs-lookup"><span data-stu-id="15d1c-113">Binary</span></span>|<span data-ttu-id="15d1c-114">Ключ, используемый для шифрования содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="15d1c-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="15d1c-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="15d1c-115">initializationVector</span></span>|<span data-ttu-id="15d1c-116">Binary</span><span class="sxs-lookup"><span data-stu-id="15d1c-116">Binary</span></span>|<span data-ttu-id="15d1c-117">Вектор инициализации, используемый для алгоритма шифрования.</span><span class="sxs-lookup"><span data-stu-id="15d1c-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="15d1c-118">mac</span><span class="sxs-lookup"><span data-stu-id="15d1c-118">mac</span></span>|<span data-ttu-id="15d1c-119">Binary</span><span class="sxs-lookup"><span data-stu-id="15d1c-119">Binary</span></span>|<span data-ttu-id="15d1c-120">Хэш зашифрованного содержимого файла + IV (хэш содержимого).</span><span class="sxs-lookup"><span data-stu-id="15d1c-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="15d1c-121">macKey</span><span class="sxs-lookup"><span data-stu-id="15d1c-121">macKey</span></span>|<span data-ttu-id="15d1c-122">Binary</span><span class="sxs-lookup"><span data-stu-id="15d1c-122">Binary</span></span>|<span data-ttu-id="15d1c-123">Ключ для получения свойства mac.</span><span class="sxs-lookup"><span data-stu-id="15d1c-123">The key used to get mac.</span></span>|
|<span data-ttu-id="15d1c-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="15d1c-124">profileIdentifier</span></span>|<span data-ttu-id="15d1c-125">String</span><span class="sxs-lookup"><span data-stu-id="15d1c-125">String</span></span>|<span data-ttu-id="15d1c-126">Идентификатор профиля.</span><span class="sxs-lookup"><span data-stu-id="15d1c-126">The the profile identifier.</span></span>|
|<span data-ttu-id="15d1c-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="15d1c-127">fileDigest</span></span>|<span data-ttu-id="15d1c-128">Binary</span><span class="sxs-lookup"><span data-stu-id="15d1c-128">Binary</span></span>|<span data-ttu-id="15d1c-129">Дайджест файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="15d1c-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="15d1c-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="15d1c-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="15d1c-131">String</span><span class="sxs-lookup"><span data-stu-id="15d1c-131">String</span></span>|<span data-ttu-id="15d1c-132">Алгоритм дайджеста файла.</span><span class="sxs-lookup"><span data-stu-id="15d1c-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15d1c-133">Связи</span><span class="sxs-lookup"><span data-stu-id="15d1c-133">Relationships</span></span>
<span data-ttu-id="15d1c-134">Нет</span><span class="sxs-lookup"><span data-stu-id="15d1c-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15d1c-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="15d1c-135">JSON Representation</span></span>
<span data-ttu-id="15d1c-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="15d1c-136">Here is a JSON representation of the resource.</span></span>
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



