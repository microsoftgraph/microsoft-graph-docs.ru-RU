---
title: Тип ресурса Апплогколлектиондовнлоаддетаилс
description: Н/Д
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3449e1f1a2b8651cea407690019d458d5ac24fa9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30147756"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="6e0d9-103">Тип ресурса Апплогколлектиондовнлоаддетаилс</span><span class="sxs-lookup"><span data-stu-id="6e0d9-103">appLogCollectionDownloadDetails resource type</span></span>

> <span data-ttu-id="6e0d9-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6e0d9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e0d9-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6e0d9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e0d9-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="6e0d9-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6e0d9-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6e0d9-107">Properties</span></span>
|<span data-ttu-id="6e0d9-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6e0d9-108">Property</span></span>|<span data-ttu-id="6e0d9-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6e0d9-109">Type</span></span>|<span data-ttu-id="6e0d9-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6e0d9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6e0d9-111">Довнлоадурл</span><span class="sxs-lookup"><span data-stu-id="6e0d9-111">downloadUrl</span></span>|<span data-ttu-id="6e0d9-112">String</span><span class="sxs-lookup"><span data-stu-id="6e0d9-112">String</span></span>|<span data-ttu-id="6e0d9-113">Скачать URL-адрес SAS для завершенного Апплогуплоадрекуест</span><span class="sxs-lookup"><span data-stu-id="6e0d9-113">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="6e0d9-114">Декриптионкэй</span><span class="sxs-lookup"><span data-stu-id="6e0d9-114">decryptionKey</span></span>|<span data-ttu-id="6e0d9-115">String</span><span class="sxs-lookup"><span data-stu-id="6e0d9-115">String</span></span>|<span data-ttu-id="6e0d9-116">Декриптионкэй как строка</span><span class="sxs-lookup"><span data-stu-id="6e0d9-116">DecryptionKey as string</span></span>|
|<span data-ttu-id="6e0d9-117">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="6e0d9-117">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="6e0d9-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="6e0d9-118">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="6e0d9-119">Декриптионалгорисм для контента.</span><span class="sxs-lookup"><span data-stu-id="6e0d9-119">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="6e0d9-120">Возможные значения: `aes256`.</span><span class="sxs-lookup"><span data-stu-id="6e0d9-120">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6e0d9-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="6e0d9-121">Relationships</span></span>
<span data-ttu-id="6e0d9-122">Нет</span><span class="sxs-lookup"><span data-stu-id="6e0d9-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6e0d9-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6e0d9-123">JSON Representation</span></span>
<span data-ttu-id="6e0d9-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6e0d9-124">Here is a JSON representation of the resource.</span></span>
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




