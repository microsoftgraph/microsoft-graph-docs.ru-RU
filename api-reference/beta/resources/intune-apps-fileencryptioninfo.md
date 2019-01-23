---
title: Тип ресурса fileEncryptionInfo
description: Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 074bf24638bf0ba7d613399e1b8894de7f30dfbb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410898"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="b0bd5-103">Тип ресурса fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="b0bd5-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="b0bd5-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b0bd5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b0bd5-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b0bd5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0bd5-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="b0bd5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0bd5-107">Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="b0bd5-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="b0bd5-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b0bd5-108">Properties</span></span>
|<span data-ttu-id="b0bd5-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b0bd5-109">Property</span></span>|<span data-ttu-id="b0bd5-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b0bd5-110">Type</span></span>|<span data-ttu-id="b0bd5-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b0bd5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0bd5-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="b0bd5-112">encryptionKey</span></span>|<span data-ttu-id="b0bd5-113">Binary</span><span class="sxs-lookup"><span data-stu-id="b0bd5-113">Binary</span></span>|<span data-ttu-id="b0bd5-114">Ключ, используемый для шифрования содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="b0bd5-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="b0bd5-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="b0bd5-115">initializationVector</span></span>|<span data-ttu-id="b0bd5-116">Binary</span><span class="sxs-lookup"><span data-stu-id="b0bd5-116">Binary</span></span>|<span data-ttu-id="b0bd5-117">Вектор инициализации, используемый для алгоритма шифрования.</span><span class="sxs-lookup"><span data-stu-id="b0bd5-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="b0bd5-118">mac</span><span class="sxs-lookup"><span data-stu-id="b0bd5-118">mac</span></span>|<span data-ttu-id="b0bd5-119">Binary</span><span class="sxs-lookup"><span data-stu-id="b0bd5-119">Binary</span></span>|<span data-ttu-id="b0bd5-120">Хэш зашифрованного содержимого файла + IV (хэш содержимого).</span><span class="sxs-lookup"><span data-stu-id="b0bd5-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="b0bd5-121">macKey</span><span class="sxs-lookup"><span data-stu-id="b0bd5-121">macKey</span></span>|<span data-ttu-id="b0bd5-122">Binary</span><span class="sxs-lookup"><span data-stu-id="b0bd5-122">Binary</span></span>|<span data-ttu-id="b0bd5-123">Ключ для получения свойства mac.</span><span class="sxs-lookup"><span data-stu-id="b0bd5-123">The key used to get mac.</span></span>|
|<span data-ttu-id="b0bd5-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="b0bd5-124">profileIdentifier</span></span>|<span data-ttu-id="b0bd5-125">String</span><span class="sxs-lookup"><span data-stu-id="b0bd5-125">String</span></span>|<span data-ttu-id="b0bd5-126">Идентификатор профиля.</span><span class="sxs-lookup"><span data-stu-id="b0bd5-126">The the profile identifier.</span></span>|
|<span data-ttu-id="b0bd5-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="b0bd5-127">fileDigest</span></span>|<span data-ttu-id="b0bd5-128">Binary</span><span class="sxs-lookup"><span data-stu-id="b0bd5-128">Binary</span></span>|<span data-ttu-id="b0bd5-129">Дайджест файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="b0bd5-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="b0bd5-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="b0bd5-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="b0bd5-131">String</span><span class="sxs-lookup"><span data-stu-id="b0bd5-131">String</span></span>|<span data-ttu-id="b0bd5-132">Алгоритм дайджеста файла.</span><span class="sxs-lookup"><span data-stu-id="b0bd5-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0bd5-133">Связи</span><span class="sxs-lookup"><span data-stu-id="b0bd5-133">Relationships</span></span>
<span data-ttu-id="b0bd5-134">Нет</span><span class="sxs-lookup"><span data-stu-id="b0bd5-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0bd5-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b0bd5-135">JSON Representation</span></span>
<span data-ttu-id="b0bd5-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b0bd5-136">Here is a JSON representation of the resource.</span></span>
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




