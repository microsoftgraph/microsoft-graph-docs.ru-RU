---
title: Тип ресурса edgeSearchEngineCustom
description: Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c1f97de9b4665769ea4e9731045603664673f64f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/21/2019
ms.locfileid: "30165732"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="65c9e-103">Тип ресурса edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="65c9e-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="65c9e-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="65c9e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65c9e-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="65c9e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65c9e-106">Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.</span><span class="sxs-lookup"><span data-stu-id="65c9e-106">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="65c9e-107">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="65c9e-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="65c9e-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="65c9e-108">Properties</span></span>
|<span data-ttu-id="65c9e-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="65c9e-109">Property</span></span>|<span data-ttu-id="65c9e-110">Тип</span><span class="sxs-lookup"><span data-stu-id="65c9e-110">Type</span></span>|<span data-ttu-id="65c9e-111">Описание</span><span class="sxs-lookup"><span data-stu-id="65c9e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65c9e-112">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="65c9e-112">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="65c9e-113">String</span><span class="sxs-lookup"><span data-stu-id="65c9e-113">String</span></span>|<span data-ttu-id="65c9e-114">Указывает на HTTPS-ссылку, содержащую XML-файл OpenSearch, в котором указаны по крайней мере краткое имя и URL-адрес поисковой системы.</span><span class="sxs-lookup"><span data-stu-id="65c9e-114">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="65c9e-115">Связи</span><span class="sxs-lookup"><span data-stu-id="65c9e-115">Relationships</span></span>
<span data-ttu-id="65c9e-116">Нет</span><span class="sxs-lookup"><span data-stu-id="65c9e-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65c9e-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="65c9e-117">JSON Representation</span></span>
<span data-ttu-id="65c9e-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="65c9e-118">Here is a JSON representation of the resource.</span></span>
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




