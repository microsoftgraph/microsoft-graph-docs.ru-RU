---
title: Тип ресурса Апплогколлектиондовнлоаддетаилс
description: Пока не задокументировано.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 95201bf8fcaf6c4b7efe1a3c552ff4a26c93dd39
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319267"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="e4ecd-103">Тип ресурса Апплогколлектиондовнлоаддетаилс</span><span class="sxs-lookup"><span data-stu-id="e4ecd-103">appLogCollectionDownloadDetails resource type</span></span>

> <span data-ttu-id="e4ecd-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e4ecd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4ecd-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e4ecd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4ecd-106">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e4ecd-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e4ecd-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="e4ecd-107">Properties</span></span>
|<span data-ttu-id="e4ecd-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="e4ecd-108">Property</span></span>|<span data-ttu-id="e4ecd-109">Тип</span><span class="sxs-lookup"><span data-stu-id="e4ecd-109">Type</span></span>|<span data-ttu-id="e4ecd-110">Описание</span><span class="sxs-lookup"><span data-stu-id="e4ecd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4ecd-111">довнлоадурл</span><span class="sxs-lookup"><span data-stu-id="e4ecd-111">downloadUrl</span></span>|<span data-ttu-id="e4ecd-112">String</span><span class="sxs-lookup"><span data-stu-id="e4ecd-112">String</span></span>|<span data-ttu-id="e4ecd-113">Скачать URL-адрес SAS для завершенного Апплогуплоадрекуест</span><span class="sxs-lookup"><span data-stu-id="e4ecd-113">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="e4ecd-114">декриптионкэй</span><span class="sxs-lookup"><span data-stu-id="e4ecd-114">decryptionKey</span></span>|<span data-ttu-id="e4ecd-115">String</span><span class="sxs-lookup"><span data-stu-id="e4ecd-115">String</span></span>|<span data-ttu-id="e4ecd-116">Декриптионкэй как строка</span><span class="sxs-lookup"><span data-stu-id="e4ecd-116">DecryptionKey as string</span></span>|
|<span data-ttu-id="e4ecd-117">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="e4ecd-117">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="e4ecd-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="e4ecd-118">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="e4ecd-119">Декриптионалгорисм для контента.</span><span class="sxs-lookup"><span data-stu-id="e4ecd-119">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="e4ecd-120">Возможные значения: `aes256`.</span><span class="sxs-lookup"><span data-stu-id="e4ecd-120">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4ecd-121">Отношения</span><span class="sxs-lookup"><span data-stu-id="e4ecd-121">Relationships</span></span>
<span data-ttu-id="e4ecd-122">Нет</span><span class="sxs-lookup"><span data-stu-id="e4ecd-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e4ecd-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e4ecd-123">JSON Representation</span></span>
<span data-ttu-id="e4ecd-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e4ecd-124">Here is a JSON representation of the resource.</span></span>
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



