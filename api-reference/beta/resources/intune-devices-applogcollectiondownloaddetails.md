---
title: Тип ресурса appLogCollectionDownloadDetails
description: Н/Д
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6946b3cd1aa60c4025859bd8d41d2dc4775bf39d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430568"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="c0ae9-103">Тип ресурса appLogCollectionDownloadDetails</span><span class="sxs-lookup"><span data-stu-id="c0ae9-103">appLogCollectionDownloadDetails resource type</span></span>

> <span data-ttu-id="c0ae9-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="c0ae9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c0ae9-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="c0ae9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0ae9-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c0ae9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0ae9-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="c0ae9-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="c0ae9-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c0ae9-108">Properties</span></span>
|<span data-ttu-id="c0ae9-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c0ae9-109">Property</span></span>|<span data-ttu-id="c0ae9-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c0ae9-110">Type</span></span>|<span data-ttu-id="c0ae9-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c0ae9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0ae9-112">downloadUrl</span><span class="sxs-lookup"><span data-stu-id="c0ae9-112">downloadUrl</span></span>|<span data-ttu-id="c0ae9-113">String</span><span class="sxs-lookup"><span data-stu-id="c0ae9-113">String</span></span>|<span data-ttu-id="c0ae9-114">URL-адрес SAS загрузки для завершения AppLogUploadRequest</span><span class="sxs-lookup"><span data-stu-id="c0ae9-114">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="c0ae9-115">decryptionKey</span><span class="sxs-lookup"><span data-stu-id="c0ae9-115">decryptionKey</span></span>|<span data-ttu-id="c0ae9-116">String</span><span class="sxs-lookup"><span data-stu-id="c0ae9-116">String</span></span>|<span data-ttu-id="c0ae9-117">DecryptionKey как строка</span><span class="sxs-lookup"><span data-stu-id="c0ae9-117">DecryptionKey as string</span></span>|
|<span data-ttu-id="c0ae9-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="c0ae9-118">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="c0ae9-119">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="c0ae9-119">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="c0ae9-120">DecryptionAlgorithm для содержимого.</span><span class="sxs-lookup"><span data-stu-id="c0ae9-120">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="c0ae9-121">Возможные значения: `aes256`.</span><span class="sxs-lookup"><span data-stu-id="c0ae9-121">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c0ae9-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="c0ae9-122">Relationships</span></span>
<span data-ttu-id="c0ae9-123">Нет</span><span class="sxs-lookup"><span data-stu-id="c0ae9-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c0ae9-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c0ae9-124">JSON Representation</span></span>
<span data-ttu-id="c0ae9-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c0ae9-125">Here is a JSON representation of the resource.</span></span>
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




