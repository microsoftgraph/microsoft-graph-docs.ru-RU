---
title: Тип ресурса userRegistrationMethodCount
description: Количество пользователей, зарегистрированных для метода проверки подлинности.
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: b61cb0448c131fc49df43154522e587644d13dc6
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052626"
---
# <a name="userregistrationmethodcount-resource-type"></a><span data-ttu-id="66fe0-103">Тип ресурса userRegistrationMethodCount</span><span class="sxs-lookup"><span data-stu-id="66fe0-103">userRegistrationMethodCount resource type</span></span>

<span data-ttu-id="66fe0-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66fe0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="66fe0-105">Количество пользователей, зарегистрированных для метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="66fe0-105">Number of users registered for an authentication method.</span></span>

## <a name="properties"></a><span data-ttu-id="66fe0-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="66fe0-106">Properties</span></span>
|<span data-ttu-id="66fe0-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="66fe0-107">Property</span></span>|<span data-ttu-id="66fe0-108">Тип</span><span class="sxs-lookup"><span data-stu-id="66fe0-108">Type</span></span>|<span data-ttu-id="66fe0-109">Описание</span><span class="sxs-lookup"><span data-stu-id="66fe0-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66fe0-110">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="66fe0-110">authenticationMethod</span></span>|<span data-ttu-id="66fe0-111">String</span><span class="sxs-lookup"><span data-stu-id="66fe0-111">String</span></span>|<span data-ttu-id="66fe0-112">Имя метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="66fe0-112">Name of authentication method.</span></span>|
|<span data-ttu-id="66fe0-113">userCount</span><span class="sxs-lookup"><span data-stu-id="66fe0-113">userCount</span></span>|<span data-ttu-id="66fe0-114">Int64</span><span class="sxs-lookup"><span data-stu-id="66fe0-114">Int64</span></span>|<span data-ttu-id="66fe0-115">Количество зарегистрированных пользователей.</span><span class="sxs-lookup"><span data-stu-id="66fe0-115">Number of users registered.</span></span>|

## <a name="relationships"></a><span data-ttu-id="66fe0-116">Связи</span><span class="sxs-lookup"><span data-stu-id="66fe0-116">Relationships</span></span>
<span data-ttu-id="66fe0-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="66fe0-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="66fe0-118">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="66fe0-118">JSON representation</span></span>
<span data-ttu-id="66fe0-119">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="66fe0-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationMethodCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationMethodCount",
  "authenticationMethod": "String",
  "userCount": "Integer"
}
```