---
title: Тип ресурса Апплогколлектиондовнлоаддетаилс
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d4b9ca36f1b9324aac50a808e2ba8fe6db398d4
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943195"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="c6bb6-103">Тип ресурса Апплогколлектиондовнлоаддетаилс</span><span class="sxs-lookup"><span data-stu-id="c6bb6-103">appLogCollectionDownloadDetails resource type</span></span>

> <span data-ttu-id="c6bb6-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c6bb6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6bb6-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c6bb6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6bb6-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c6bb6-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c6bb6-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c6bb6-107">Properties</span></span>
|<span data-ttu-id="c6bb6-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c6bb6-108">Property</span></span>|<span data-ttu-id="c6bb6-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c6bb6-109">Type</span></span>|<span data-ttu-id="c6bb6-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c6bb6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6bb6-111">Довнлоадурл</span><span class="sxs-lookup"><span data-stu-id="c6bb6-111">downloadUrl</span></span>|<span data-ttu-id="c6bb6-112">Строка</span><span class="sxs-lookup"><span data-stu-id="c6bb6-112">String</span></span>|<span data-ttu-id="c6bb6-113">Скачать URL-адрес SAS для завершенного Апплогуплоадрекуест</span><span class="sxs-lookup"><span data-stu-id="c6bb6-113">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="c6bb6-114">Декриптионкэй</span><span class="sxs-lookup"><span data-stu-id="c6bb6-114">decryptionKey</span></span>|<span data-ttu-id="c6bb6-115">Строка</span><span class="sxs-lookup"><span data-stu-id="c6bb6-115">String</span></span>|<span data-ttu-id="c6bb6-116">Декриптионкэй как строка</span><span class="sxs-lookup"><span data-stu-id="c6bb6-116">DecryptionKey as string</span></span>|
|<span data-ttu-id="c6bb6-117">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="c6bb6-117">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="c6bb6-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="c6bb6-118">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="c6bb6-119">Декриптионалгорисм для контента.</span><span class="sxs-lookup"><span data-stu-id="c6bb6-119">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="c6bb6-120">Возможные значения: `aes256`.</span><span class="sxs-lookup"><span data-stu-id="c6bb6-120">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c6bb6-121">Связи</span><span class="sxs-lookup"><span data-stu-id="c6bb6-121">Relationships</span></span>
<span data-ttu-id="c6bb6-122">Нет</span><span class="sxs-lookup"><span data-stu-id="c6bb6-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c6bb6-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c6bb6-123">JSON Representation</span></span>
<span data-ttu-id="c6bb6-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c6bb6-124">Here is a JSON representation of the resource.</span></span>
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




