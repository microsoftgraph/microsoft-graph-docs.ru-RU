---
title: Тип ресурса fileEncryptionInfo
description: Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9a2236e2c63703ea5af2662d5b0f4594e7888799
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552179"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="3f2cc-103">Тип ресурса fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="3f2cc-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="3f2cc-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="3f2cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f2cc-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3f2cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f2cc-106">Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="3f2cc-106">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="3f2cc-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="3f2cc-107">Properties</span></span>
|<span data-ttu-id="3f2cc-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="3f2cc-108">Property</span></span>|<span data-ttu-id="3f2cc-109">Тип</span><span class="sxs-lookup"><span data-stu-id="3f2cc-109">Type</span></span>|<span data-ttu-id="3f2cc-110">Описание</span><span class="sxs-lookup"><span data-stu-id="3f2cc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f2cc-111">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="3f2cc-111">encryptionKey</span></span>|<span data-ttu-id="3f2cc-112">Двоичный</span><span class="sxs-lookup"><span data-stu-id="3f2cc-112">Binary</span></span>|<span data-ttu-id="3f2cc-113">Ключ, используемый для шифрования содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="3f2cc-113">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="3f2cc-114">initializationVector</span><span class="sxs-lookup"><span data-stu-id="3f2cc-114">initializationVector</span></span>|<span data-ttu-id="3f2cc-115">Двоичный</span><span class="sxs-lookup"><span data-stu-id="3f2cc-115">Binary</span></span>|<span data-ttu-id="3f2cc-116">Вектор инициализации, используемый для алгоритма шифрования.</span><span class="sxs-lookup"><span data-stu-id="3f2cc-116">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="3f2cc-117">mac</span><span class="sxs-lookup"><span data-stu-id="3f2cc-117">mac</span></span>|<span data-ttu-id="3f2cc-118">Двоичный</span><span class="sxs-lookup"><span data-stu-id="3f2cc-118">Binary</span></span>|<span data-ttu-id="3f2cc-119">Хэш зашифрованного содержимого файла + IV (хэш содержимого).</span><span class="sxs-lookup"><span data-stu-id="3f2cc-119">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="3f2cc-120">macKey</span><span class="sxs-lookup"><span data-stu-id="3f2cc-120">macKey</span></span>|<span data-ttu-id="3f2cc-121">Двоичный</span><span class="sxs-lookup"><span data-stu-id="3f2cc-121">Binary</span></span>|<span data-ttu-id="3f2cc-122">Ключ для получения свойства mac.</span><span class="sxs-lookup"><span data-stu-id="3f2cc-122">The key used to get mac.</span></span>|
|<span data-ttu-id="3f2cc-123">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="3f2cc-123">profileIdentifier</span></span>|<span data-ttu-id="3f2cc-124">String</span><span class="sxs-lookup"><span data-stu-id="3f2cc-124">String</span></span>|<span data-ttu-id="3f2cc-125">Идентификатор профиля.</span><span class="sxs-lookup"><span data-stu-id="3f2cc-125">The the profile identifier.</span></span>|
|<span data-ttu-id="3f2cc-126">fileDigest</span><span class="sxs-lookup"><span data-stu-id="3f2cc-126">fileDigest</span></span>|<span data-ttu-id="3f2cc-127">Binary</span><span class="sxs-lookup"><span data-stu-id="3f2cc-127">Binary</span></span>|<span data-ttu-id="3f2cc-128">Дайджест файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="3f2cc-128">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="3f2cc-129">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="3f2cc-129">fileDigestAlgorithm</span></span>|<span data-ttu-id="3f2cc-130">String</span><span class="sxs-lookup"><span data-stu-id="3f2cc-130">String</span></span>|<span data-ttu-id="3f2cc-131">Алгоритм дайджеста файла.</span><span class="sxs-lookup"><span data-stu-id="3f2cc-131">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f2cc-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="3f2cc-132">Relationships</span></span>
<span data-ttu-id="3f2cc-133">Нет</span><span class="sxs-lookup"><span data-stu-id="3f2cc-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f2cc-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3f2cc-134">JSON Representation</span></span>
<span data-ttu-id="3f2cc-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3f2cc-135">Here is a JSON representation of the resource.</span></span>
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





