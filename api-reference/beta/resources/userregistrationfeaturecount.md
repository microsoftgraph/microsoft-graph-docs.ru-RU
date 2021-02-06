---
title: Тип ресурса userRegistrationFeatureCount
description: Количество пользователей, зарегистрированных или способных выполнять многофакторную проверку подлинности, Self-Service и проверку подлинности без пароля.
author: danielwood95
localization_priority: Normal
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 7c73d9cd17d5bf13eb5f8899e0d1e9dc6e27af67
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132946"
---
# <a name="userregistrationfeaturecount-resource-type"></a><span data-ttu-id="9877c-103">Тип ресурса userRegistrationFeatureCount</span><span class="sxs-lookup"><span data-stu-id="9877c-103">userRegistrationFeatureCount resource type</span></span>

<span data-ttu-id="9877c-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9877c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9877c-105">Представляет количество пользователей, зарегистрированных или способных выполнять многофакторную проверку подлинности, Self-Service и проверку подлинности без пароля.</span><span class="sxs-lookup"><span data-stu-id="9877c-105">Represents the number of users registered or capable for Multi-Factor Authentication, Self-Service Password Reset and Passwordless Authentication.</span></span>

## <a name="properties"></a><span data-ttu-id="9877c-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="9877c-106">Properties</span></span>
|<span data-ttu-id="9877c-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="9877c-107">Property</span></span>|<span data-ttu-id="9877c-108">Тип</span><span class="sxs-lookup"><span data-stu-id="9877c-108">Type</span></span>|<span data-ttu-id="9877c-109">Описание</span><span class="sxs-lookup"><span data-stu-id="9877c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9877c-110">feature</span><span class="sxs-lookup"><span data-stu-id="9877c-110">feature</span></span>|<span data-ttu-id="9877c-111">authenticationMethodFeature</span><span class="sxs-lookup"><span data-stu-id="9877c-111">authenticationMethodFeature</span></span>|<span data-ttu-id="9877c-112">Количество пользователей, зарегистрированных или способных использовать многофакторную проверку подлинности, Self-Service и проверку подлинности без пароля.</span><span class="sxs-lookup"><span data-stu-id="9877c-112">Number of users registered or capable for Multi-Factor Authentication, Self-Service Password Reset and Passwordless Authentication.</span></span> <span data-ttu-id="9877c-113">Возможные значения: `ssprRegistered`, `ssprEnabled`, `ssprCapable`, `passwordlessCapable`, `mfaCapable`.</span><span class="sxs-lookup"><span data-stu-id="9877c-113">Possible values are: `ssprRegistered`, `ssprEnabled`, `ssprCapable`, `passwordlessCapable`, `mfaCapable`.</span></span>|
|<span data-ttu-id="9877c-114">userCount</span><span class="sxs-lookup"><span data-stu-id="9877c-114">userCount</span></span>|<span data-ttu-id="9877c-115">Int64</span><span class="sxs-lookup"><span data-stu-id="9877c-115">Int64</span></span>|<span data-ttu-id="9877c-116">Количество пользователей.</span><span class="sxs-lookup"><span data-stu-id="9877c-116">Number of users.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9877c-117">Связи</span><span class="sxs-lookup"><span data-stu-id="9877c-117">Relationships</span></span>
<span data-ttu-id="9877c-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9877c-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9877c-119">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="9877c-119">JSON representation</span></span>
<span data-ttu-id="9877c-120">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="9877c-120">The following is a JSON representation of the resource.</span></span>
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
