---
title: Тип ресурса edgeSearchEngineCustom
description: Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 69395d09c01c1b92f2ae3ee1abf26eeff09618f8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425983"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="914af-103">Тип ресурса edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="914af-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="914af-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="914af-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="914af-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="914af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="914af-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="914af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="914af-107">Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.</span><span class="sxs-lookup"><span data-stu-id="914af-107">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="914af-108">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="914af-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="914af-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="914af-109">Properties</span></span>
|<span data-ttu-id="914af-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="914af-110">Property</span></span>|<span data-ttu-id="914af-111">Тип</span><span class="sxs-lookup"><span data-stu-id="914af-111">Type</span></span>|<span data-ttu-id="914af-112">Описание</span><span class="sxs-lookup"><span data-stu-id="914af-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="914af-113">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="914af-113">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="914af-114">String</span><span class="sxs-lookup"><span data-stu-id="914af-114">String</span></span>|<span data-ttu-id="914af-115">Указывает на HTTPS-ссылку, содержащую XML-файл OpenSearch, в котором указаны по крайней мере краткое имя и URL-адрес поисковой системы.</span><span class="sxs-lookup"><span data-stu-id="914af-115">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="914af-116">Связи</span><span class="sxs-lookup"><span data-stu-id="914af-116">Relationships</span></span>
<span data-ttu-id="914af-117">Нет</span><span class="sxs-lookup"><span data-stu-id="914af-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="914af-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="914af-118">JSON Representation</span></span>
<span data-ttu-id="914af-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="914af-119">Here is a JSON representation of the resource.</span></span>
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




