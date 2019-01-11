---
title: Тип ресурса fileEncryptionInfo
description: Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ed56f695da8dece64702472cd3822603e02dd8b6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840693"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="891c0-103">Тип ресурса fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="891c0-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="891c0-104">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="891c0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="891c0-105">Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="891c0-105">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="891c0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="891c0-106">Properties</span></span>
|<span data-ttu-id="891c0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="891c0-107">Property</span></span>|<span data-ttu-id="891c0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="891c0-108">Type</span></span>|<span data-ttu-id="891c0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="891c0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="891c0-110">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="891c0-110">encryptionKey</span></span>|<span data-ttu-id="891c0-111">Binary</span><span class="sxs-lookup"><span data-stu-id="891c0-111">Binary</span></span>|<span data-ttu-id="891c0-112">Ключ, используемый для шифрования содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="891c0-112">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="891c0-113">initializationVector</span><span class="sxs-lookup"><span data-stu-id="891c0-113">initializationVector</span></span>|<span data-ttu-id="891c0-114">Binary</span><span class="sxs-lookup"><span data-stu-id="891c0-114">Binary</span></span>|<span data-ttu-id="891c0-115">Вектор инициализации, используемый для алгоритма шифрования.</span><span class="sxs-lookup"><span data-stu-id="891c0-115">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="891c0-116">mac</span><span class="sxs-lookup"><span data-stu-id="891c0-116">mac</span></span>|<span data-ttu-id="891c0-117">Binary</span><span class="sxs-lookup"><span data-stu-id="891c0-117">Binary</span></span>|<span data-ttu-id="891c0-118">Хэш зашифрованного содержимого файла + IV (хэш содержимого).</span><span class="sxs-lookup"><span data-stu-id="891c0-118">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="891c0-119">macKey</span><span class="sxs-lookup"><span data-stu-id="891c0-119">macKey</span></span>|<span data-ttu-id="891c0-120">Binary</span><span class="sxs-lookup"><span data-stu-id="891c0-120">Binary</span></span>|<span data-ttu-id="891c0-121">Ключ для получения свойства mac.</span><span class="sxs-lookup"><span data-stu-id="891c0-121">The key used to get mac.</span></span>|
|<span data-ttu-id="891c0-122">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="891c0-122">profileIdentifier</span></span>|<span data-ttu-id="891c0-123">String</span><span class="sxs-lookup"><span data-stu-id="891c0-123">String</span></span>|<span data-ttu-id="891c0-124">Идентификатор профиля.</span><span class="sxs-lookup"><span data-stu-id="891c0-124">The the profile identifier.</span></span>|
|<span data-ttu-id="891c0-125">fileDigest</span><span class="sxs-lookup"><span data-stu-id="891c0-125">fileDigest</span></span>|<span data-ttu-id="891c0-126">Binary</span><span class="sxs-lookup"><span data-stu-id="891c0-126">Binary</span></span>|<span data-ttu-id="891c0-127">Дайджест файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="891c0-127">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="891c0-128">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="891c0-128">fileDigestAlgorithm</span></span>|<span data-ttu-id="891c0-129">String</span><span class="sxs-lookup"><span data-stu-id="891c0-129">String</span></span>|<span data-ttu-id="891c0-130">Алгоритм дайджеста файла.</span><span class="sxs-lookup"><span data-stu-id="891c0-130">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="891c0-131">Связи</span><span class="sxs-lookup"><span data-stu-id="891c0-131">Relationships</span></span>
<span data-ttu-id="891c0-132">Нет</span><span class="sxs-lookup"><span data-stu-id="891c0-132">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="891c0-133">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="891c0-133">JSON Representation</span></span>
<span data-ttu-id="891c0-134">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="891c0-134">Here is a JSON representation of the resource.</span></span>
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



