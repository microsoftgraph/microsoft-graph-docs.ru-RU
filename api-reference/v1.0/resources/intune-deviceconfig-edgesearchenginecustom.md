---
title: Тип ресурса edgeSearchEngineCustom
description: Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2d48793eed6930b21defdb1f8f7aa921cdece2e5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532541"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="c4665-103">Тип ресурса edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="c4665-103">edgeSearchEngineCustom resource type</span></span>

<span data-ttu-id="c4665-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c4665-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c4665-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="c4665-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4665-106">Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.</span><span class="sxs-lookup"><span data-stu-id="c4665-106">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="c4665-107">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="c4665-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c4665-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="c4665-108">Properties</span></span>
|<span data-ttu-id="c4665-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="c4665-109">Property</span></span>|<span data-ttu-id="c4665-110">Тип</span><span class="sxs-lookup"><span data-stu-id="c4665-110">Type</span></span>|<span data-ttu-id="c4665-111">Описание</span><span class="sxs-lookup"><span data-stu-id="c4665-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4665-112">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="c4665-112">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="c4665-113">String</span><span class="sxs-lookup"><span data-stu-id="c4665-113">String</span></span>|<span data-ttu-id="c4665-114">Указывает на HTTPS-ссылку, содержащую XML-файл OpenSearch, в котором указаны по крайней мере краткое имя и URL-адрес поисковой системы.</span><span class="sxs-lookup"><span data-stu-id="c4665-114">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4665-115">Связи</span><span class="sxs-lookup"><span data-stu-id="c4665-115">Relationships</span></span>
<span data-ttu-id="c4665-116">Нет</span><span class="sxs-lookup"><span data-stu-id="c4665-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c4665-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="c4665-117">JSON Representation</span></span>
<span data-ttu-id="c4665-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c4665-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngineCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineCustom",
  "edgeSearchEngineOpenSearchXmlUrl": "String"
}
```




