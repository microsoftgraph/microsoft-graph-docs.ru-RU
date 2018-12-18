---
title: Тип ресурса windows10AssociatedApps
description: Определение приложения связанного 10 Windows.
author: tfitzmac
ms.openlocfilehash: a990d3b1f9b2b33a1e98fd30f5dea4da7fbf4ae8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344830"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="b2095-103">Тип ресурса windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="b2095-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="b2095-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="b2095-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2095-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="b2095-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b2095-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="b2095-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2095-107">Определение приложения связанного 10 Windows.</span><span class="sxs-lookup"><span data-stu-id="b2095-107">Windows 10 Associated Application definition.</span></span>
## <a name="properties"></a><span data-ttu-id="b2095-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="b2095-108">Properties</span></span>
|<span data-ttu-id="b2095-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="b2095-109">Property</span></span>|<span data-ttu-id="b2095-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b2095-110">Type</span></span>|<span data-ttu-id="b2095-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b2095-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2095-112">Тип</span><span class="sxs-lookup"><span data-stu-id="b2095-112">appType</span></span>|[<span data-ttu-id="b2095-113">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="b2095-113">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="b2095-114">Тип приложения.</span><span class="sxs-lookup"><span data-stu-id="b2095-114">Application type.</span></span> <span data-ttu-id="b2095-115">Возможные значения: `desktop`, `universal`.</span><span class="sxs-lookup"><span data-stu-id="b2095-115">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="b2095-116">идентификатор</span><span class="sxs-lookup"><span data-stu-id="b2095-116">identifier</span></span>|<span data-ttu-id="b2095-117">String.</span><span class="sxs-lookup"><span data-stu-id="b2095-117">String</span></span>|<span data-ttu-id="b2095-118">Идентификатор.</span><span class="sxs-lookup"><span data-stu-id="b2095-118">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b2095-119">Связи</span><span class="sxs-lookup"><span data-stu-id="b2095-119">Relationships</span></span>
<span data-ttu-id="b2095-120">Нет</span><span class="sxs-lookup"><span data-stu-id="b2095-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b2095-121">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="b2095-121">JSON Representation</span></span>
<span data-ttu-id="b2095-122">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="b2095-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AssociatedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AssociatedApps",
  "appType": "String",
  "identifier": "String"
}
```





