---
title: Тип ресурса edgeSearchEngineCustom
description: Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ebfd7cf46399e9033ff3a0df592b0a112eb2e726
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49199023"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="18c53-103">Тип ресурса edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="18c53-103">edgeSearchEngineCustom resource type</span></span>

<span data-ttu-id="18c53-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18c53-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18c53-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="18c53-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="18c53-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="18c53-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18c53-107">Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.</span><span class="sxs-lookup"><span data-stu-id="18c53-107">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>


<span data-ttu-id="18c53-108">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="18c53-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="18c53-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="18c53-109">Properties</span></span>
|<span data-ttu-id="18c53-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="18c53-110">Property</span></span>|<span data-ttu-id="18c53-111">Тип</span><span class="sxs-lookup"><span data-stu-id="18c53-111">Type</span></span>|<span data-ttu-id="18c53-112">Описание</span><span class="sxs-lookup"><span data-stu-id="18c53-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18c53-113">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="18c53-113">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="18c53-114">String</span><span class="sxs-lookup"><span data-stu-id="18c53-114">String</span></span>|<span data-ttu-id="18c53-115">Указывает на HTTPS-ссылку, содержащую XML-файл OpenSearch, в котором указаны по крайней мере краткое имя и URL-адрес поисковой системы.</span><span class="sxs-lookup"><span data-stu-id="18c53-115">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="18c53-116">Связи</span><span class="sxs-lookup"><span data-stu-id="18c53-116">Relationships</span></span>
<span data-ttu-id="18c53-117">Нет</span><span class="sxs-lookup"><span data-stu-id="18c53-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="18c53-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="18c53-118">JSON Representation</span></span>
<span data-ttu-id="18c53-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="18c53-119">Here is a JSON representation of the resource.</span></span>
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




