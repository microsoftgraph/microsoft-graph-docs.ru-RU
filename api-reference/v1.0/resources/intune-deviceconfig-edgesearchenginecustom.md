---
title: Тип ресурса edgeSearchEngineCustom
description: Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 523a2de33619886997cbcb052079bbf2937c9d48
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541229"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="ca9f1-103">Тип ресурса edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="ca9f1-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="ca9f1-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="ca9f1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca9f1-105">Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.</span><span class="sxs-lookup"><span data-stu-id="ca9f1-105">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="ca9f1-106">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="ca9f1-106">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ca9f1-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="ca9f1-107">Properties</span></span>
|<span data-ttu-id="ca9f1-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="ca9f1-108">Property</span></span>|<span data-ttu-id="ca9f1-109">Тип</span><span class="sxs-lookup"><span data-stu-id="ca9f1-109">Type</span></span>|<span data-ttu-id="ca9f1-110">Описание</span><span class="sxs-lookup"><span data-stu-id="ca9f1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca9f1-111">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="ca9f1-111">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="ca9f1-112">String</span><span class="sxs-lookup"><span data-stu-id="ca9f1-112">String</span></span>|<span data-ttu-id="ca9f1-113">Указывает на HTTPS-ссылку, содержащую XML-файл OpenSearch, в котором указаны по крайней мере краткое имя и URL-адрес поисковой системы.</span><span class="sxs-lookup"><span data-stu-id="ca9f1-113">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ca9f1-114">Отношения</span><span class="sxs-lookup"><span data-stu-id="ca9f1-114">Relationships</span></span>
<span data-ttu-id="ca9f1-115">Нет</span><span class="sxs-lookup"><span data-stu-id="ca9f1-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca9f1-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="ca9f1-116">JSON Representation</span></span>
<span data-ttu-id="ca9f1-117">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ca9f1-117">Here is a JSON representation of the resource.</span></span>
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



