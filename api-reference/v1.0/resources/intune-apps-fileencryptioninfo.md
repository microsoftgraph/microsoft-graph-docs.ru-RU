---
title: Тип ресурса fileEncryptionInfo
description: Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a0859447e06b7264f5018e575c047a283d02dc34
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532850"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="2ba7d-103">Тип ресурса fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="2ba7d-103">fileEncryptionInfo resource type</span></span>

<span data-ttu-id="2ba7d-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ba7d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ba7d-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="2ba7d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ba7d-106">Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="2ba7d-106">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="2ba7d-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="2ba7d-107">Properties</span></span>
|<span data-ttu-id="2ba7d-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="2ba7d-108">Property</span></span>|<span data-ttu-id="2ba7d-109">Тип</span><span class="sxs-lookup"><span data-stu-id="2ba7d-109">Type</span></span>|<span data-ttu-id="2ba7d-110">Описание</span><span class="sxs-lookup"><span data-stu-id="2ba7d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ba7d-111">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="2ba7d-111">encryptionKey</span></span>|<span data-ttu-id="2ba7d-112">Binary</span><span class="sxs-lookup"><span data-stu-id="2ba7d-112">Binary</span></span>|<span data-ttu-id="2ba7d-113">Ключ, используемый для шифрования содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="2ba7d-113">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="2ba7d-114">initializationVector</span><span class="sxs-lookup"><span data-stu-id="2ba7d-114">initializationVector</span></span>|<span data-ttu-id="2ba7d-115">Binary</span><span class="sxs-lookup"><span data-stu-id="2ba7d-115">Binary</span></span>|<span data-ttu-id="2ba7d-116">Вектор инициализации, используемый для алгоритма шифрования.</span><span class="sxs-lookup"><span data-stu-id="2ba7d-116">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="2ba7d-117">mac</span><span class="sxs-lookup"><span data-stu-id="2ba7d-117">mac</span></span>|<span data-ttu-id="2ba7d-118">Binary</span><span class="sxs-lookup"><span data-stu-id="2ba7d-118">Binary</span></span>|<span data-ttu-id="2ba7d-119">Хэш зашифрованного содержимого файла + IV (хэш содержимого).</span><span class="sxs-lookup"><span data-stu-id="2ba7d-119">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="2ba7d-120">macKey</span><span class="sxs-lookup"><span data-stu-id="2ba7d-120">macKey</span></span>|<span data-ttu-id="2ba7d-121">Binary</span><span class="sxs-lookup"><span data-stu-id="2ba7d-121">Binary</span></span>|<span data-ttu-id="2ba7d-122">Ключ для получения свойства mac.</span><span class="sxs-lookup"><span data-stu-id="2ba7d-122">The key used to get mac.</span></span>|
|<span data-ttu-id="2ba7d-123">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="2ba7d-123">profileIdentifier</span></span>|<span data-ttu-id="2ba7d-124">Строка</span><span class="sxs-lookup"><span data-stu-id="2ba7d-124">String</span></span>|<span data-ttu-id="2ba7d-125">Идентификатор профиля.</span><span class="sxs-lookup"><span data-stu-id="2ba7d-125">The profile identifier.</span></span>|
|<span data-ttu-id="2ba7d-126">fileDigest</span><span class="sxs-lookup"><span data-stu-id="2ba7d-126">fileDigest</span></span>|<span data-ttu-id="2ba7d-127">Binary</span><span class="sxs-lookup"><span data-stu-id="2ba7d-127">Binary</span></span>|<span data-ttu-id="2ba7d-128">Дайджест файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="2ba7d-128">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="2ba7d-129">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="2ba7d-129">fileDigestAlgorithm</span></span>|<span data-ttu-id="2ba7d-130">String</span><span class="sxs-lookup"><span data-stu-id="2ba7d-130">String</span></span>|<span data-ttu-id="2ba7d-131">Алгоритм дайджеста файла.</span><span class="sxs-lookup"><span data-stu-id="2ba7d-131">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ba7d-132">Связи</span><span class="sxs-lookup"><span data-stu-id="2ba7d-132">Relationships</span></span>
<span data-ttu-id="2ba7d-133">Нет</span><span class="sxs-lookup"><span data-stu-id="2ba7d-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ba7d-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2ba7d-134">JSON Representation</span></span>
<span data-ttu-id="2ba7d-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2ba7d-135">Here is a JSON representation of the resource.</span></span>
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




