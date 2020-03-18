---
title: Тип ресурса Апплогколлектиондовнлоаддетаилс
description: Пока не задокументировано.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dd570fbe0b999ab6d93d5d37d03f8689b5d9b405
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785248"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="6688e-103">Тип ресурса Апплогколлектиондовнлоаддетаилс</span><span class="sxs-lookup"><span data-stu-id="6688e-103">appLogCollectionDownloadDetails resource type</span></span>

> <span data-ttu-id="6688e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6688e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6688e-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6688e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6688e-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6688e-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6688e-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6688e-107">Properties</span></span>
|<span data-ttu-id="6688e-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6688e-108">Property</span></span>|<span data-ttu-id="6688e-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6688e-109">Type</span></span>|<span data-ttu-id="6688e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6688e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6688e-111">довнлоадурл</span><span class="sxs-lookup"><span data-stu-id="6688e-111">downloadUrl</span></span>|<span data-ttu-id="6688e-112">String</span><span class="sxs-lookup"><span data-stu-id="6688e-112">String</span></span>|<span data-ttu-id="6688e-113">Скачать URL-адрес SAS для завершенного Апплогуплоадрекуест</span><span class="sxs-lookup"><span data-stu-id="6688e-113">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="6688e-114">декриптионкэй</span><span class="sxs-lookup"><span data-stu-id="6688e-114">decryptionKey</span></span>|<span data-ttu-id="6688e-115">String</span><span class="sxs-lookup"><span data-stu-id="6688e-115">String</span></span>|<span data-ttu-id="6688e-116">Декриптионкэй как строка</span><span class="sxs-lookup"><span data-stu-id="6688e-116">DecryptionKey as string</span></span>|
|<span data-ttu-id="6688e-117">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="6688e-117">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="6688e-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="6688e-118">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="6688e-119">Декриптионалгорисм для контента.</span><span class="sxs-lookup"><span data-stu-id="6688e-119">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="6688e-120">Возможные значения: `aes256`.</span><span class="sxs-lookup"><span data-stu-id="6688e-120">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6688e-121">Связи</span><span class="sxs-lookup"><span data-stu-id="6688e-121">Relationships</span></span>
<span data-ttu-id="6688e-122">Нет</span><span class="sxs-lookup"><span data-stu-id="6688e-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6688e-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6688e-123">JSON Representation</span></span>
<span data-ttu-id="6688e-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6688e-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appLogCollectionDownloadDetails"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appLogCollectionDownloadDetails",
  "downloadUrl": "String",
  "decryptionKey": "String",
  "appLogDecryptionAlgorithm": "String"
}
```



