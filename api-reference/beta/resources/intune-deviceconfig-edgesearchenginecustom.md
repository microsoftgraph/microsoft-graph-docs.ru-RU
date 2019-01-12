---
title: Тип ресурса edgeSearchEngineCustom
description: Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8171c293610efc790eadc0619c99fe604d6c933b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932891"
---
# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="2de65-103">Тип ресурса edgeSearchEngineCustom</span><span class="sxs-lookup"><span data-stu-id="2de65-103">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="2de65-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="2de65-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2de65-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="2de65-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2de65-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="2de65-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2de65-107">Позволяет ИТ-администраторам устанавливать поисковую систему по умолчанию для устройств под управлением MDM.</span><span class="sxs-lookup"><span data-stu-id="2de65-107">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="2de65-108">Наследуется от [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span><span class="sxs-lookup"><span data-stu-id="2de65-108">Inherits from [edgeSearchEngineBase](../resources/intune-deviceconfig-edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2de65-109">Свойства</span><span class="sxs-lookup"><span data-stu-id="2de65-109">Properties</span></span>
|<span data-ttu-id="2de65-110">Свойство</span><span class="sxs-lookup"><span data-stu-id="2de65-110">Property</span></span>|<span data-ttu-id="2de65-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2de65-111">Type</span></span>|<span data-ttu-id="2de65-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2de65-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2de65-113">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="2de65-113">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="2de65-114">String</span><span class="sxs-lookup"><span data-stu-id="2de65-114">String</span></span>|<span data-ttu-id="2de65-115">Указывает на HTTPS-ссылку, содержащую XML-файл OpenSearch, в котором указаны по крайней мере краткое имя и URL-адрес поисковой системы.</span><span class="sxs-lookup"><span data-stu-id="2de65-115">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2de65-116">Связи</span><span class="sxs-lookup"><span data-stu-id="2de65-116">Relationships</span></span>
<span data-ttu-id="2de65-117">Нет</span><span class="sxs-lookup"><span data-stu-id="2de65-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2de65-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="2de65-118">JSON Representation</span></span>
<span data-ttu-id="2de65-119">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="2de65-119">Here is a JSON representation of the resource.</span></span>
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





