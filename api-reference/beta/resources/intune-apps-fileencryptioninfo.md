---
title: Тип ресурса fileEncryptionInfo
description: Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 18ff7b9d64473048b6d1d45069ab19549c83e0df
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27960121"
---
# <a name="fileencryptioninfo-resource-type"></a><span data-ttu-id="eac06-103">Тип ресурса fileEncryptionInfo</span><span class="sxs-lookup"><span data-stu-id="eac06-103">fileEncryptionInfo resource type</span></span>

> <span data-ttu-id="eac06-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="eac06-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eac06-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="eac06-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eac06-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="eac06-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eac06-107">Содержит свойства сведений о шифровании файлов для версии содержимого бизнес-приложения.</span><span class="sxs-lookup"><span data-stu-id="eac06-107">Contains properties for file encryption information for the content version of a line of business app.</span></span>
## <a name="properties"></a><span data-ttu-id="eac06-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="eac06-108">Properties</span></span>
|<span data-ttu-id="eac06-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="eac06-109">Property</span></span>|<span data-ttu-id="eac06-110">Тип</span><span class="sxs-lookup"><span data-stu-id="eac06-110">Type</span></span>|<span data-ttu-id="eac06-111">Описание</span><span class="sxs-lookup"><span data-stu-id="eac06-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eac06-112">encryptionKey</span><span class="sxs-lookup"><span data-stu-id="eac06-112">encryptionKey</span></span>|<span data-ttu-id="eac06-113">Binary</span><span class="sxs-lookup"><span data-stu-id="eac06-113">Binary</span></span>|<span data-ttu-id="eac06-114">Ключ, используемый для шифрования содержимого файла.</span><span class="sxs-lookup"><span data-stu-id="eac06-114">The key used to encrypt the file content.</span></span>|
|<span data-ttu-id="eac06-115">initializationVector</span><span class="sxs-lookup"><span data-stu-id="eac06-115">initializationVector</span></span>|<span data-ttu-id="eac06-116">Binary</span><span class="sxs-lookup"><span data-stu-id="eac06-116">Binary</span></span>|<span data-ttu-id="eac06-117">Вектор инициализации, используемый для алгоритма шифрования.</span><span class="sxs-lookup"><span data-stu-id="eac06-117">The initialization vector used for the encryption algorithm.</span></span>|
|<span data-ttu-id="eac06-118">mac</span><span class="sxs-lookup"><span data-stu-id="eac06-118">mac</span></span>|<span data-ttu-id="eac06-119">Binary</span><span class="sxs-lookup"><span data-stu-id="eac06-119">Binary</span></span>|<span data-ttu-id="eac06-120">Хэш зашифрованного содержимого файла + IV (хэш содержимого).</span><span class="sxs-lookup"><span data-stu-id="eac06-120">The hash of the encrypted file content + IV (content hash).</span></span>|
|<span data-ttu-id="eac06-121">macKey</span><span class="sxs-lookup"><span data-stu-id="eac06-121">macKey</span></span>|<span data-ttu-id="eac06-122">Binary</span><span class="sxs-lookup"><span data-stu-id="eac06-122">Binary</span></span>|<span data-ttu-id="eac06-123">Ключ для получения свойства mac.</span><span class="sxs-lookup"><span data-stu-id="eac06-123">The key used to get mac.</span></span>|
|<span data-ttu-id="eac06-124">profileIdentifier</span><span class="sxs-lookup"><span data-stu-id="eac06-124">profileIdentifier</span></span>|<span data-ttu-id="eac06-125">String</span><span class="sxs-lookup"><span data-stu-id="eac06-125">String</span></span>|<span data-ttu-id="eac06-126">Идентификатор профиля.</span><span class="sxs-lookup"><span data-stu-id="eac06-126">The the profile identifier.</span></span>|
|<span data-ttu-id="eac06-127">fileDigest</span><span class="sxs-lookup"><span data-stu-id="eac06-127">fileDigest</span></span>|<span data-ttu-id="eac06-128">Binary</span><span class="sxs-lookup"><span data-stu-id="eac06-128">Binary</span></span>|<span data-ttu-id="eac06-129">Дайджест файла до шифрования.</span><span class="sxs-lookup"><span data-stu-id="eac06-129">The file digest prior to encryption.</span></span>|
|<span data-ttu-id="eac06-130">fileDigestAlgorithm</span><span class="sxs-lookup"><span data-stu-id="eac06-130">fileDigestAlgorithm</span></span>|<span data-ttu-id="eac06-131">String</span><span class="sxs-lookup"><span data-stu-id="eac06-131">String</span></span>|<span data-ttu-id="eac06-132">Алгоритм дайджеста файла.</span><span class="sxs-lookup"><span data-stu-id="eac06-132">The file digest algorithm.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eac06-133">Связи</span><span class="sxs-lookup"><span data-stu-id="eac06-133">Relationships</span></span>
<span data-ttu-id="eac06-134">Нет</span><span class="sxs-lookup"><span data-stu-id="eac06-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eac06-135">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="eac06-135">JSON Representation</span></span>
<span data-ttu-id="eac06-136">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="eac06-136">Here is a JSON representation of the resource.</span></span>
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





