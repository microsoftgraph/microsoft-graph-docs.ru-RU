---
title: Тип ресурса Апплогколлектиондовнлоаддетаилс
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dade0c3a266e8cba801a8e88dacebda6bbd2d197
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465258"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="cdc11-103">Тип ресурса Апплогколлектиондовнлоаддетаилс</span><span class="sxs-lookup"><span data-stu-id="cdc11-103">appLogCollectionDownloadDetails resource type</span></span>

<span data-ttu-id="cdc11-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdc11-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cdc11-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cdc11-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdc11-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cdc11-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdc11-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="cdc11-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="cdc11-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cdc11-108">Properties</span></span>
|<span data-ttu-id="cdc11-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cdc11-109">Property</span></span>|<span data-ttu-id="cdc11-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cdc11-110">Type</span></span>|<span data-ttu-id="cdc11-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cdc11-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdc11-112">довнлоадурл</span><span class="sxs-lookup"><span data-stu-id="cdc11-112">downloadUrl</span></span>|<span data-ttu-id="cdc11-113">String</span><span class="sxs-lookup"><span data-stu-id="cdc11-113">String</span></span>|<span data-ttu-id="cdc11-114">Скачать URL-адрес SAS для завершенного Апплогуплоадрекуест</span><span class="sxs-lookup"><span data-stu-id="cdc11-114">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="cdc11-115">декриптионкэй</span><span class="sxs-lookup"><span data-stu-id="cdc11-115">decryptionKey</span></span>|<span data-ttu-id="cdc11-116">String</span><span class="sxs-lookup"><span data-stu-id="cdc11-116">String</span></span>|<span data-ttu-id="cdc11-117">Декриптионкэй как строка</span><span class="sxs-lookup"><span data-stu-id="cdc11-117">DecryptionKey as string</span></span>|
|<span data-ttu-id="cdc11-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="cdc11-118">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="cdc11-119">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="cdc11-119">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="cdc11-120">Декриптионалгорисм для контента.</span><span class="sxs-lookup"><span data-stu-id="cdc11-120">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="cdc11-121">Возможные значения: `aes256`.</span><span class="sxs-lookup"><span data-stu-id="cdc11-121">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cdc11-122">Отношения</span><span class="sxs-lookup"><span data-stu-id="cdc11-122">Relationships</span></span>
<span data-ttu-id="cdc11-123">Нет</span><span class="sxs-lookup"><span data-stu-id="cdc11-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cdc11-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cdc11-124">JSON Representation</span></span>
<span data-ttu-id="cdc11-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cdc11-125">Here is a JSON representation of the resource.</span></span>
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



