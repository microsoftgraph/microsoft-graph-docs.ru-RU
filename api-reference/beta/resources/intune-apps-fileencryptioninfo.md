---
title: Тип ресурса fileEncryptionInfo
description: Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 03d8adbbf43b38bfc7d13bec2db09c2be8c3b2ca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868973"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="07290-103">Тип ресурса fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="07290-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="07290-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="07290-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="07290-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07290-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="07290-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="07290-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="07290-107">Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="07290-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="07290-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="07290-108">Properties</span></span>
|<span data-ttu-id="07290-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="07290-109">Property</span></span>|<span data-ttu-id="07290-110">Тип</span><span class="sxs-lookup"><span data-stu-id="07290-110">Type</span></span>|<span data-ttu-id="07290-111">Описание</span><span class="sxs-lookup"><span data-stu-id="07290-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07290-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="07290-112">encryptionKey</span></span>|<span data-ttu-id="07290-113">Binary</span><span class="sxs-lookup"><span data-stu-id="07290-113">Binary</span></span>|<span data-ttu-id="07290-114">Ключ, используемый для шифрования содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="07290-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="07290-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="07290-115">initializationVector</span></span>|<span data-ttu-id="07290-116">Binary</span><span class="sxs-lookup"><span data-stu-id="07290-116">Binary</span></span>|<span data-ttu-id="07290-117">Вектор инициализации, используемый для алгоритма шифрования.</span><span class="sxs-lookup"><span data-stu-id="07290-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="07290-118">mac</span><span class="sxs-lookup"><span data-stu-id="07290-118">mac</span></span>|<span data-ttu-id="07290-119">Binary</span><span class="sxs-lookup"><span data-stu-id="07290-119">Binary</span></span>|<span data-ttu-id="07290-120">Хэш зашифрованного содержимого файла + IV (хэш содержимого).</span><span class="sxs-lookup"><span data-stu-id="07290-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="07290-121">macKey</span><span class="sxs-lookup"><span data-stu-id="07290-121">macKey</span></span>|<span data-ttu-id="07290-122">Binary</span><span class="sxs-lookup"><span data-stu-id="07290-122">Binary</span></span>|<span data-ttu-id="07290-123">Ключ для получения свойства mac.</span><span class="sxs-lookup"><span data-stu-id="07290-123">The key used to get mac.</span></span>|
|<span data-ttu-id="07290-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="07290-124">profileIdentifier</span></span>|<span data-ttu-id="07290-125">String</span><span class="sxs-lookup"><span data-stu-id="07290-125">String</span></span>|<span data-ttu-id="07290-126">Идентификатор профиля.</span><span class="sxs-lookup"><span data-stu-id="07290-126">The the profile identifier.</span></span>|
|<span data-ttu-id="07290-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="07290-127">fileDigest</span></span>|<span data-ttu-id="07290-128">Binary</span><span class="sxs-lookup"><span data-stu-id="07290-128">Binary</span></span>|<span data-ttu-id="07290-129">Дайджест файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="07290-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="07290-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="07290-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="07290-131">String</span><span class="sxs-lookup"><span data-stu-id="07290-131">String</span></span>|<span data-ttu-id="07290-132">Алгоритм дайджеста файла.</span><span class="sxs-lookup"><span data-stu-id="07290-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="07290-133">Связи</span><span class="sxs-lookup"><span data-stu-id="07290-133">Relationships</span></span>
<span data-ttu-id="07290-134">Нет</span><span class="sxs-lookup"><span data-stu-id="07290-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="07290-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="07290-135">JSON Representation</span></span>
<span data-ttu-id="07290-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="07290-136">Here is a JSON representation of the resource.</span></span>
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





