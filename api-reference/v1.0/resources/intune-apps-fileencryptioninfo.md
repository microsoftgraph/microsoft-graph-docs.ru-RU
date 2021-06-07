---
title: Тип ресурса fileEncryptionInfo
description: Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7f22c1d25b45b31cf682ad95d573fe3b41534dc9
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755611"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="a322c-103">Тип ресурса fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="a322c-103">fileEncryptionInfo resource type</span></span>

<span data-ttu-id="a322c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a322c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a322c-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="a322c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a322c-106">Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="a322c-106">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="a322c-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="a322c-107">Properties</span></span>
|<span data-ttu-id="a322c-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="a322c-108">Property</span></span>|<span data-ttu-id="a322c-109">Тип</span><span class="sxs-lookup"><span data-stu-id="a322c-109">Type</span></span>|<span data-ttu-id="a322c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="a322c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a322c-111">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="a322c-111">encryptionKey</span></span>|<span data-ttu-id="a322c-112">Binary</span><span class="sxs-lookup"><span data-stu-id="a322c-112">Binary</span></span>|<span data-ttu-id="a322c-113">Ключ, используемый для шифрования содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="a322c-113">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="a322c-114">initializationVector</span><span class="sxs-lookup"><span data-stu-id="a322c-114">initializationVector</span></span>|<span data-ttu-id="a322c-115">Binary</span><span class="sxs-lookup"><span data-stu-id="a322c-115">Binary</span></span>|<span data-ttu-id="a322c-116">Вектор инициализации, используемый для алгоритма шифрования.</span><span class="sxs-lookup"><span data-stu-id="a322c-116">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="a322c-117">mac</span><span class="sxs-lookup"><span data-stu-id="a322c-117">mac</span></span>|<span data-ttu-id="a322c-118">Binary</span><span class="sxs-lookup"><span data-stu-id="a322c-118">Binary</span></span>|<span data-ttu-id="a322c-119">Хэш зашифрованного содержимого файла + IV (хэш содержимого).</span><span class="sxs-lookup"><span data-stu-id="a322c-119">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="a322c-120">macKey</span><span class="sxs-lookup"><span data-stu-id="a322c-120">macKey</span></span>|<span data-ttu-id="a322c-121">Binary</span><span class="sxs-lookup"><span data-stu-id="a322c-121">Binary</span></span>|<span data-ttu-id="a322c-122">Ключ для получения свойства mac.</span><span class="sxs-lookup"><span data-stu-id="a322c-122">The key used to get mac.</span></span>|
|<span data-ttu-id="a322c-123">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="a322c-123">profileIdentifier</span></span>|<span data-ttu-id="a322c-124">String</span><span class="sxs-lookup"><span data-stu-id="a322c-124">String</span></span>|<span data-ttu-id="a322c-125">Идентификатор профиля.</span><span class="sxs-lookup"><span data-stu-id="a322c-125">The the profile identifier.</span></span>|
|<span data-ttu-id="a322c-126">fileDigest</span><span class="sxs-lookup"><span data-stu-id="a322c-126">fileDigest</span></span>|<span data-ttu-id="a322c-127">Binary</span><span class="sxs-lookup"><span data-stu-id="a322c-127">Binary</span></span>|<span data-ttu-id="a322c-128">Дайджест файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="a322c-128">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="a322c-129">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="a322c-129">fileDigestAlgorithm</span></span>|<span data-ttu-id="a322c-130">String</span><span class="sxs-lookup"><span data-stu-id="a322c-130">String</span></span>|<span data-ttu-id="a322c-131">Алгоритм дайджеста файла.</span><span class="sxs-lookup"><span data-stu-id="a322c-131">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a322c-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="a322c-132">Relationships</span></span>
<span data-ttu-id="a322c-133">Нет</span><span class="sxs-lookup"><span data-stu-id="a322c-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a322c-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a322c-134">JSON Representation</span></span>
<span data-ttu-id="a322c-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="a322c-135">Here is a JSON representation of the resource.</span></span>
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




