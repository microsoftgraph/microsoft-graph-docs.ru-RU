---
title: Тип ресурса edgeSearchEngineCustom
description: Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2858b1b4ce96655965b4e990682352819d50d9a1
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/02/2019
ms.locfileid: "37359329"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="42d48-103">Тип ресурса edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="42d48-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="42d48-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="42d48-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42d48-105">Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.</span><span class="sxs-lookup"><span data-stu-id="42d48-105">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="42d48-106">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="42d48-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="42d48-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="42d48-107">Properties</span></span>
|<span data-ttu-id="42d48-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="42d48-108">Property</span></span>|<span data-ttu-id="42d48-109">Тип</span><span class="sxs-lookup"><span data-stu-id="42d48-109">Type</span></span>|<span data-ttu-id="42d48-110">Описание</span><span class="sxs-lookup"><span data-stu-id="42d48-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42d48-111">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="42d48-111">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="42d48-112">String</span><span class="sxs-lookup"><span data-stu-id="42d48-112">String</span></span>|<span data-ttu-id="42d48-113">Указывает на HTTPS-ссылку, содержащую XML-файл OpenSearch, в котором указаны по крайней мере краткое имя и URL-адрес поисковой системы.</span><span class="sxs-lookup"><span data-stu-id="42d48-113">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42d48-114">Связи</span><span class="sxs-lookup"><span data-stu-id="42d48-114">Relationships</span></span>
<span data-ttu-id="42d48-115">Нет</span><span class="sxs-lookup"><span data-stu-id="42d48-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42d48-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="42d48-116">JSON Representation</span></span>
<span data-ttu-id="42d48-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="42d48-117">Here is a JSON representation of the resource.</span></span>
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




