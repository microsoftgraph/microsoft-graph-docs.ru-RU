---
title: Тип ресурса Сугжестеденроллментлимит
description: Ресурс Сугжестеденроллментлимит представляет Рекомендуемое предельное значение регистрации при наличии типа регистрации.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b54c89a946f6a5b5b8dd66a8e4146f6e12793d89
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728888"
---
# <a name="suggestedenrollmentlimit-resource-type"></a><span data-ttu-id="6d881-103">Тип ресурса Сугжестеденроллментлимит</span><span class="sxs-lookup"><span data-stu-id="6d881-103">suggestedEnrollmentLimit resource type</span></span>

<span data-ttu-id="6d881-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d881-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d881-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="6d881-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d881-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="6d881-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d881-107">Ресурс Сугжестеденроллментлимит представляет Рекомендуемое предельное значение регистрации при наличии типа регистрации.</span><span class="sxs-lookup"><span data-stu-id="6d881-107">The suggestedEnrollmentLimit resource represents the suggested enrollment limit when given an enrollment type.</span></span>

## <a name="properties"></a><span data-ttu-id="6d881-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="6d881-108">Properties</span></span>
|<span data-ttu-id="6d881-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="6d881-109">Property</span></span>|<span data-ttu-id="6d881-110">Тип</span><span class="sxs-lookup"><span data-stu-id="6d881-110">Type</span></span>|<span data-ttu-id="6d881-111">Описание</span><span class="sxs-lookup"><span data-stu-id="6d881-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d881-112">сугжестеддаилилимит</span><span class="sxs-lookup"><span data-stu-id="6d881-112">suggestedDailyLimit</span></span>|<span data-ttu-id="6d881-113">Int32</span><span class="sxs-lookup"><span data-stu-id="6d881-113">Int32</span></span>|<span data-ttu-id="6d881-114">Предполагаемое количество заявок в течение дня</span><span class="sxs-lookup"><span data-stu-id="6d881-114">The suggested enrollment limit within a day</span></span>|

## <a name="relationships"></a><span data-ttu-id="6d881-115">Связи</span><span class="sxs-lookup"><span data-stu-id="6d881-115">Relationships</span></span>
<span data-ttu-id="6d881-116">Нет</span><span class="sxs-lookup"><span data-stu-id="6d881-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6d881-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6d881-117">JSON Representation</span></span>
<span data-ttu-id="6d881-118">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6d881-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.suggestedEnrollmentLimit"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.suggestedEnrollmentLimit",
  "suggestedDailyLimit": 1024
}
```





