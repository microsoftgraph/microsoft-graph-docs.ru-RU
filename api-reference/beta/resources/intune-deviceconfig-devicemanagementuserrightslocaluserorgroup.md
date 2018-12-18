---
title: Тип ресурса deviceManagementUserRightsLocalUserOrGroup
description: Представляет сведения для локального пользователя или группы, используемые для настройки прав пользователя.
author: tfitzmac
ms.openlocfilehash: baabd2f3bb9e3bce44d172cd83f61f57c5c2c98d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27303733"
---
# <a name="devicemanagementuserrightslocaluserorgroup-resource-type"></a><span data-ttu-id="d6115-103">Тип ресурса deviceManagementUserRightsLocalUserOrGroup</span><span class="sxs-lookup"><span data-stu-id="d6115-103">deviceManagementUserRightsLocalUserOrGroup resource type</span></span>

> <span data-ttu-id="d6115-104">**Важно:** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="d6115-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6115-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="d6115-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6115-106">**Примечание.** Для настройки элементов управления и политик Intune с помощью API Microsoft Graph по-прежнему требуется, чтобы клиент [лицензировал](https://go.microsoft.com/fwlink/?linkid=839381) Intune надлежащим образом.</span><span class="sxs-lookup"><span data-stu-id="d6115-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6115-107">Представляет сведения для локального пользователя или группы, используемые для настройки прав пользователя.</span><span class="sxs-lookup"><span data-stu-id="d6115-107">Represents information for a local user or group used for user rights setting.</span></span>
## <a name="properties"></a><span data-ttu-id="d6115-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d6115-108">Properties</span></span>
|<span data-ttu-id="d6115-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d6115-109">Property</span></span>|<span data-ttu-id="d6115-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d6115-110">Type</span></span>|<span data-ttu-id="d6115-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d6115-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6115-112">name</span><span class="sxs-lookup"><span data-stu-id="d6115-112">name</span></span>|<span data-ttu-id="d6115-113">Строка</span><span class="sxs-lookup"><span data-stu-id="d6115-113">String</span></span>|<span data-ttu-id="d6115-114">Имя этого локального пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="d6115-114">The name of this local user or group.</span></span>|
|<span data-ttu-id="d6115-115">описание</span><span class="sxs-lookup"><span data-stu-id="d6115-115">description</span></span>|<span data-ttu-id="d6115-116">Строка</span><span class="sxs-lookup"><span data-stu-id="d6115-116">String</span></span>|<span data-ttu-id="d6115-117">Описание администратора локального пользователя или группы.</span><span class="sxs-lookup"><span data-stu-id="d6115-117">Admin’s description of this local user or group.</span></span>|
|<span data-ttu-id="d6115-118">Класс securityIdentifier</span><span class="sxs-lookup"><span data-stu-id="d6115-118">securityIdentifier</span></span>|<span data-ttu-id="d6115-119">String.</span><span class="sxs-lookup"><span data-stu-id="d6115-119">String</span></span>|<span data-ttu-id="d6115-120">Идентификатор безопасности этого локального пользователя или группы (например \* S-1-5-32-544).</span><span class="sxs-lookup"><span data-stu-id="d6115-120">The security identifier of this local user or group (e.g. \*S-1-5-32-544).</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6115-121">Связи</span><span class="sxs-lookup"><span data-stu-id="d6115-121">Relationships</span></span>
<span data-ttu-id="d6115-122">Нет</span><span class="sxs-lookup"><span data-stu-id="d6115-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d6115-123">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d6115-123">JSON Representation</span></span>
<span data-ttu-id="d6115-124">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d6115-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementUserRightsLocalUserOrGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementUserRightsLocalUserOrGroup",
  "name": "String",
  "description": "String",
  "securityIdentifier": "String"
}
```





