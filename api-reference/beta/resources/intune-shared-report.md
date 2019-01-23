---
title: Тип ресурса report
description: Описание отчетов ресурсов из Microsoft Graph API для Intune, которая поддерживает несколько рабочих процессов.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 098c20b2460324c4975533902e1b71fde1af41c5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407475"
---
# <a name="report-resource-type"></a><span data-ttu-id="9d714-103">Тип ресурса report</span><span class="sxs-lookup"><span data-stu-id="9d714-103">report resource type</span></span>

> <span data-ttu-id="9d714-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="9d714-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d714-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="9d714-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9d714-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="9d714-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d714-107">Возвращает содержимое контексту, включая:</span><span class="sxs-lookup"><span data-stu-id="9d714-107">Returns the content appropriate for the context, including:</span></span>

- <span data-ttu-id="9d714-108">Отчеты журнала профиля конфигурации устройства.</span><span class="sxs-lookup"><span data-stu-id="9d714-108">Device Configuration profile history reports.</span></span>
- <span data-ttu-id="9d714-109">Отчеты заявок через Интернет.</span><span class="sxs-lookup"><span data-stu-id="9d714-109">Enrollment failure reports.</span></span>

## <a name="properties"></a><span data-ttu-id="9d714-110">Свойства</span><span class="sxs-lookup"><span data-stu-id="9d714-110">Properties</span></span>
|<span data-ttu-id="9d714-111">Свойство</span><span class="sxs-lookup"><span data-stu-id="9d714-111">Property</span></span>|<span data-ttu-id="9d714-112">Тип</span><span class="sxs-lookup"><span data-stu-id="9d714-112">Type</span></span>|<span data-ttu-id="9d714-113">Описание</span><span class="sxs-lookup"><span data-stu-id="9d714-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d714-114">content</span><span class="sxs-lookup"><span data-stu-id="9d714-114">content</span></span>|<span data-ttu-id="9d714-115">Stream</span><span class="sxs-lookup"><span data-stu-id="9d714-115">Stream</span></span>|<span data-ttu-id="9d714-116">Отчет о содержимого; сведения в зависимости от типа отчета.</span><span class="sxs-lookup"><span data-stu-id="9d714-116">Report content; details vary by report type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d714-117">Отношения</span><span class="sxs-lookup"><span data-stu-id="9d714-117">Relationships</span></span>
<span data-ttu-id="9d714-118">Нет</span><span class="sxs-lookup"><span data-stu-id="9d714-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d714-119">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="9d714-119">JSON Representation</span></span>
<span data-ttu-id="9d714-120">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9d714-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.report"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.report",
  "content": "<Unknown Primitive Type Edm.Stream>"
}
```



