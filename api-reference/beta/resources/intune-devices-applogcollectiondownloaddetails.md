---
title: Тип ресурса Апплогколлектиондовнлоаддетаилс
description: Пока не задокументировано.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ced02355c4d1b0d57761c7374e46bb41d7a35558
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260070"
---
# <a name="applogcollectiondownloaddetails-resource-type"></a><span data-ttu-id="e1825-103">Тип ресурса Апплогколлектиондовнлоаддетаилс</span><span class="sxs-lookup"><span data-stu-id="e1825-103">appLogCollectionDownloadDetails resource type</span></span>

<span data-ttu-id="e1825-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1825-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e1825-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e1825-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1825-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="e1825-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1825-107">Н/Д</span><span class="sxs-lookup"><span data-stu-id="e1825-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="e1825-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e1825-108">Properties</span></span>
|<span data-ttu-id="e1825-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e1825-109">Property</span></span>|<span data-ttu-id="e1825-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e1825-110">Type</span></span>|<span data-ttu-id="e1825-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e1825-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1825-112">довнлоадурл</span><span class="sxs-lookup"><span data-stu-id="e1825-112">downloadUrl</span></span>|<span data-ttu-id="e1825-113">String</span><span class="sxs-lookup"><span data-stu-id="e1825-113">String</span></span>|<span data-ttu-id="e1825-114">Скачать URL-адрес SAS для завершенного Апплогуплоадрекуест</span><span class="sxs-lookup"><span data-stu-id="e1825-114">Download SAS Url for completed AppLogUploadRequest</span></span>|
|<span data-ttu-id="e1825-115">декриптионкэй</span><span class="sxs-lookup"><span data-stu-id="e1825-115">decryptionKey</span></span>|<span data-ttu-id="e1825-116">String</span><span class="sxs-lookup"><span data-stu-id="e1825-116">String</span></span>|<span data-ttu-id="e1825-117">Декриптионкэй как строка</span><span class="sxs-lookup"><span data-stu-id="e1825-117">DecryptionKey as string</span></span>|
|<span data-ttu-id="e1825-118">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="e1825-118">appLogDecryptionAlgorithm</span></span>|[<span data-ttu-id="e1825-119">appLogDecryptionAlgorithm</span><span class="sxs-lookup"><span data-stu-id="e1825-119">appLogDecryptionAlgorithm</span></span>](../resources/intune-devices-applogdecryptionalgorithm.md)|<span data-ttu-id="e1825-120">Декриптионалгорисм для контента.</span><span class="sxs-lookup"><span data-stu-id="e1825-120">DecryptionAlgorithm for Content.</span></span> <span data-ttu-id="e1825-121">Возможные значения: `aes256` .</span><span class="sxs-lookup"><span data-stu-id="e1825-121">Possible values are: `aes256`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1825-122">Связи</span><span class="sxs-lookup"><span data-stu-id="e1825-122">Relationships</span></span>
<span data-ttu-id="e1825-123">Нет</span><span class="sxs-lookup"><span data-stu-id="e1825-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1825-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e1825-124">JSON Representation</span></span>
<span data-ttu-id="e1825-125">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="e1825-125">Here is a JSON representation of the resource.</span></span>
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




