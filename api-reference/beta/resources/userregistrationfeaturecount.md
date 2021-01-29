---
title: Тип ресурса userRegistrationFeatureCount
description: Количество пользователей, зарегистрированных или способных использовать многофакторную проверку подлинности, Self-Service и проверку подлинности без пароля.
author: danielwood95
localization_priority: Normal
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: 0a0ad3758a74e057fa5539d3d913dd1735c88854
ms.sourcegitcommit: 90f08b197a9b13593143618c105a4049c07811b8
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052618"
---
# <a name="userregistrationfeaturecount-resource-type"></a><span data-ttu-id="ad52a-103">Тип ресурса userRegistrationFeatureCount</span><span class="sxs-lookup"><span data-stu-id="ad52a-103">userRegistrationFeatureCount resource type</span></span>

<span data-ttu-id="ad52a-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ad52a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad52a-105">Представляет количество пользователей, зарегистрированных или способных выполнять многофакторную проверку подлинности, Self-Service и проверку подлинности без пароля.</span><span class="sxs-lookup"><span data-stu-id="ad52a-105">Represents the number of users registered or capable for Multi-Factor Authentication, Self-Service Password Reset and Passwordless Authentication.</span></span>

## <a name="properties"></a><span data-ttu-id="ad52a-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="ad52a-106">Properties</span></span>
|<span data-ttu-id="ad52a-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="ad52a-107">Property</span></span>|<span data-ttu-id="ad52a-108">Тип</span><span class="sxs-lookup"><span data-stu-id="ad52a-108">Type</span></span>|<span data-ttu-id="ad52a-109">Описание</span><span class="sxs-lookup"><span data-stu-id="ad52a-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad52a-110">feature</span><span class="sxs-lookup"><span data-stu-id="ad52a-110">feature</span></span>|<span data-ttu-id="ad52a-111">authenticationMethodFeature</span><span class="sxs-lookup"><span data-stu-id="ad52a-111">authenticationMethodFeature</span></span>|<span data-ttu-id="ad52a-112">Количество пользователей, зарегистрированных или способных использовать многофакторную проверку подлинности, Self-Service и проверку подлинности без пароля.</span><span class="sxs-lookup"><span data-stu-id="ad52a-112">Number of users registered or capable for Multi-Factor Authentication, Self-Service Password Reset and Passwordless Authentication.</span></span> <span data-ttu-id="ad52a-113">Возможные значения: `ssprRegistered`, `ssprEnabled`, `ssprCapable`, `passwordlessCapable`, `mfaCapable`.</span><span class="sxs-lookup"><span data-stu-id="ad52a-113">Possible values are: `ssprRegistered`, `ssprEnabled`, `ssprCapable`, `passwordlessCapable`, `mfaCapable`.</span></span>|
|<span data-ttu-id="ad52a-114">userCount</span><span class="sxs-lookup"><span data-stu-id="ad52a-114">userCount</span></span>|<span data-ttu-id="ad52a-115">Int64</span><span class="sxs-lookup"><span data-stu-id="ad52a-115">Int64</span></span>|<span data-ttu-id="ad52a-116">Количество пользователей.</span><span class="sxs-lookup"><span data-stu-id="ad52a-116">Number of users.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ad52a-117">Связи</span><span class="sxs-lookup"><span data-stu-id="ad52a-117">Relationships</span></span>
<span data-ttu-id="ad52a-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ad52a-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad52a-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="ad52a-119">JSON representation</span></span>
<span data-ttu-id="ad52a-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="ad52a-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.userRegistrationFeatureCount"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userRegistrationFeatureCount",
  "feature": "String",
  "userCount": "Integer"
}
```
