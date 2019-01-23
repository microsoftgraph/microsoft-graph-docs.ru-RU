---
title: Тип ресурса loggedOnUser
description: Вход в систему пользователя
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6ac0ca08c6d324836e4bb9dd9951fdfe742b8b5f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395197"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="cc46c-103">Тип ресурса loggedOnUser</span><span class="sxs-lookup"><span data-stu-id="cc46c-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="cc46c-104">**Важные:** Интерфейсы API в разделе версии /beta в Microsoft Graph могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="cc46c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cc46c-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="cc46c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc46c-106">**Примечание:** Microsoft Graph API для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="cc46c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc46c-107">Вход в систему пользователя</span><span class="sxs-lookup"><span data-stu-id="cc46c-107">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="cc46c-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="cc46c-108">Properties</span></span>
|<span data-ttu-id="cc46c-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="cc46c-109">Property</span></span>|<span data-ttu-id="cc46c-110">Тип</span><span class="sxs-lookup"><span data-stu-id="cc46c-110">Type</span></span>|<span data-ttu-id="cc46c-111">Описание</span><span class="sxs-lookup"><span data-stu-id="cc46c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc46c-112">userId</span><span class="sxs-lookup"><span data-stu-id="cc46c-112">userId</span></span>|<span data-ttu-id="cc46c-113">String</span><span class="sxs-lookup"><span data-stu-id="cc46c-113">String</span></span>|<span data-ttu-id="cc46c-114">Идентификатор пользователя</span><span class="sxs-lookup"><span data-stu-id="cc46c-114">User id</span></span>|
|<span data-ttu-id="cc46c-115">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="cc46c-115">lastLogOnDateTime</span></span>|<span data-ttu-id="cc46c-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc46c-116">DateTimeOffset</span></span>|<span data-ttu-id="cc46c-117">Дата и время, при входе пользователя в систему</span><span class="sxs-lookup"><span data-stu-id="cc46c-117">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc46c-118">Отношения</span><span class="sxs-lookup"><span data-stu-id="cc46c-118">Relationships</span></span>
<span data-ttu-id="cc46c-119">Нет</span><span class="sxs-lookup"><span data-stu-id="cc46c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc46c-120">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="cc46c-120">JSON Representation</span></span>
<span data-ttu-id="cc46c-121">Ниже представлено описание ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="cc46c-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loggedOnUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loggedOnUser",
  "userId": "String",
  "lastLogOnDateTime": "String (timestamp)"
}
```




