---
title: Тип ресурса edgeSearchEngineCustom
description: Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dc0f0f7175a5b2cfb6be8f2b09b83ad263ae6050
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758864"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="3adef-103">Тип ресурса edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="3adef-103">edgeSearchEngineCustom resource type</span></span>

<span data-ttu-id="3adef-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3adef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3adef-105">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="3adef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3adef-106">Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.</span><span class="sxs-lookup"><span data-stu-id="3adef-106">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="3adef-107">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="3adef-107">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3adef-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="3adef-108">Properties</span></span>
|<span data-ttu-id="3adef-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="3adef-109">Property</span></span>|<span data-ttu-id="3adef-110">Тип</span><span class="sxs-lookup"><span data-stu-id="3adef-110">Type</span></span>|<span data-ttu-id="3adef-111">Описание</span><span class="sxs-lookup"><span data-stu-id="3adef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3adef-112">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="3adef-112">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="3adef-113">String</span><span class="sxs-lookup"><span data-stu-id="3adef-113">String</span></span>|<span data-ttu-id="3adef-114">Указывает на HTTPS-ссылку, содержащую XML-файл OpenSearch, в котором указаны по крайней мере краткое имя и URL-адрес поисковой системы.</span><span class="sxs-lookup"><span data-stu-id="3adef-114">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3adef-115">Связи</span><span class="sxs-lookup"><span data-stu-id="3adef-115">Relationships</span></span>
<span data-ttu-id="3adef-116">Нет</span><span class="sxs-lookup"><span data-stu-id="3adef-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3adef-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="3adef-117">JSON Representation</span></span>
<span data-ttu-id="3adef-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="3adef-118">Here is a JSON representation of the resource.</span></span>
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




