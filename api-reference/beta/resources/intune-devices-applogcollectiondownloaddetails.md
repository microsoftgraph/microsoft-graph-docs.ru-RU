---
title: Тип ресурса Апплогколлектиондовнлоаддетаилс
description: Пока не задокументировано.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c581b6ffe1653c2962c03c8e6fe5d27d706882d5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/11/2019
ms.locfileid: "31784742"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="e10bd-103">Тип ресурса Апплогколлектиондовнлоаддетаилс</span><span class="sxs-lookup"><span data-stu-id="e10bd-103">appLogCollectionDownloadDetails resource type</span></span>

> <span data-ttu-id="e10bd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e10bd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e10bd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e10bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e10bd-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e10bd-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e10bd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e10bd-107">Properties</span></span>
|<span data-ttu-id="e10bd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e10bd-108">Property</span></span>|<span data-ttu-id="e10bd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e10bd-109">Type</span></span>|<span data-ttu-id="e10bd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e10bd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e10bd-111">Довнлоадурл</span><span class="sxs-lookup"><span data-stu-id="e10bd-111">downloadUrl</span></span>|<span data-ttu-id="e10bd-112">String</span><span class="sxs-lookup"><span data-stu-id="e10bd-112">String</span></span>|<span data-ttu-id="e10bd-113">Скачать URL-адрес SAS для завершенного Апплогуплоадрекуест</span><span class="sxs-lookup"><span data-stu-id="e10bd-113">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="e10bd-114">Декриптионкэй</span><span class="sxs-lookup"><span data-stu-id="e10bd-114">decryptionKey</span></span>|<span data-ttu-id="e10bd-115">String</span><span class="sxs-lookup"><span data-stu-id="e10bd-115">String</span></span>|<span data-ttu-id="e10bd-116">Декриптионкэй как строка</span><span class="sxs-lookup"><span data-stu-id="e10bd-116">DecryptionKey as string</span></span>|
|<span data-ttu-id="e10bd-117">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="e10bd-117">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="e10bd-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="e10bd-118">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="e10bd-119">Декриптионалгорисм для контента.</span><span class="sxs-lookup"><span data-stu-id="e10bd-119">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="e10bd-120">Возможные значения: `aes256`.</span><span class="sxs-lookup"><span data-stu-id="e10bd-120">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e10bd-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="e10bd-121">Relationships</span></span>
<span data-ttu-id="e10bd-122">Нет</span><span class="sxs-lookup"><span data-stu-id="e10bd-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e10bd-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e10bd-123">JSON Representation</span></span>
<span data-ttu-id="e10bd-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e10bd-124">Here is a JSON representation of the resource.</span></span>
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





