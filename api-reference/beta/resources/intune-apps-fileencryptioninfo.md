---
title: Тип ресурса fileEncryptionInfo
description: Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 725a47eda88cbbdad752d73e6ea3451dcc3d140b
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991312"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="ae518-103">Тип ресурса fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="ae518-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="ae518-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="ae518-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae518-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ae518-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae518-106">Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="ae518-106">Contains properties for file encryption information for the content version of a line of business app.</span></span>

## <a name="properties"></a><span data-ttu-id="ae518-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ae518-107">Properties</span></span>
|<span data-ttu-id="ae518-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ae518-108">Property</span></span>|<span data-ttu-id="ae518-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ae518-109">Type</span></span>|<span data-ttu-id="ae518-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ae518-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae518-111">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="ae518-111">encryptionKey</span></span>|<span data-ttu-id="ae518-112">Binary</span><span class="sxs-lookup"><span data-stu-id="ae518-112">Binary</span></span>|<span data-ttu-id="ae518-113">Ключ, используемый для шифрования содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="ae518-113">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="ae518-114">initializationVector</span><span class="sxs-lookup"><span data-stu-id="ae518-114">initializationVector</span></span>|<span data-ttu-id="ae518-115">Binary</span><span class="sxs-lookup"><span data-stu-id="ae518-115">Binary</span></span>|<span data-ttu-id="ae518-116">Вектор инициализации, используемый для алгоритма шифрования.</span><span class="sxs-lookup"><span data-stu-id="ae518-116">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="ae518-117">mac</span><span class="sxs-lookup"><span data-stu-id="ae518-117">mac</span></span>|<span data-ttu-id="ae518-118">Binary</span><span class="sxs-lookup"><span data-stu-id="ae518-118">Binary</span></span>|<span data-ttu-id="ae518-119">Хэш зашифрованного содержимого файла + IV (хэш содержимого).</span><span class="sxs-lookup"><span data-stu-id="ae518-119">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="ae518-120">macKey</span><span class="sxs-lookup"><span data-stu-id="ae518-120">macKey</span></span>|<span data-ttu-id="ae518-121">Binary</span><span class="sxs-lookup"><span data-stu-id="ae518-121">Binary</span></span>|<span data-ttu-id="ae518-122">Ключ для получения свойства mac.</span><span class="sxs-lookup"><span data-stu-id="ae518-122">The key used to get mac.</span></span>|
|<span data-ttu-id="ae518-123">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="ae518-123">profileIdentifier</span></span>|<span data-ttu-id="ae518-124">String</span><span class="sxs-lookup"><span data-stu-id="ae518-124">String</span></span>|<span data-ttu-id="ae518-125">Идентификатор профиля.</span><span class="sxs-lookup"><span data-stu-id="ae518-125">The the profile identifier.</span></span>|
|<span data-ttu-id="ae518-126">fileDigest</span><span class="sxs-lookup"><span data-stu-id="ae518-126">fileDigest</span></span>|<span data-ttu-id="ae518-127">Binary</span><span class="sxs-lookup"><span data-stu-id="ae518-127">Binary</span></span>|<span data-ttu-id="ae518-128">Дайджест файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="ae518-128">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="ae518-129">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="ae518-129">fileDigestAlgorithm</span></span>|<span data-ttu-id="ae518-130">String</span><span class="sxs-lookup"><span data-stu-id="ae518-130">String</span></span>|<span data-ttu-id="ae518-131">Алгоритм дайджеста файла.</span><span class="sxs-lookup"><span data-stu-id="ae518-131">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ae518-132">Отношения</span><span class="sxs-lookup"><span data-stu-id="ae518-132">Relationships</span></span>
<span data-ttu-id="ae518-133">Нет</span><span class="sxs-lookup"><span data-stu-id="ae518-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ae518-134">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ae518-134">JSON Representation</span></span>
<span data-ttu-id="ae518-135">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ae518-135">Here is a JSON representation of the resource.</span></span>
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





