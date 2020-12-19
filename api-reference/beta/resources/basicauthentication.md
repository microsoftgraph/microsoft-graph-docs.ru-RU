---
title: Тип ресурса basicAuthentication
description: Представляет конфигурацию для использования базовой проверки подлинности в вызове API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9de5fad9746e8562f51d1ddc8fcea350c41979ed
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720442"
---
# <a name="basicauthentication-resource-type"></a><span data-ttu-id="d79fe-103">Тип ресурса basicAuthentication</span><span class="sxs-lookup"><span data-stu-id="d79fe-103">basicAuthentication resource type</span></span>

<span data-ttu-id="d79fe-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d79fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d79fe-105">Представляет конфигурацию для использования проверки подлинности HTTP Basic, которая влечет за собой имя пользователя и пароль, в вызове API.</span><span class="sxs-lookup"><span data-stu-id="d79fe-105">Represents configuration for using HTTP Basic authentication, which entails a username and password, in an API call.</span></span> <span data-ttu-id="d79fe-106">Имя пользователя и пароль отправляются в качестве загона авторизации, где находится кодированная версия username:password в кодированном коде `Basic {value}` `value` base 64.</span><span class="sxs-lookup"><span data-stu-id="d79fe-106">The username and password is sent as the Authorization header as `Basic {value}` where `value` is base 64 encoded version of username:password.</span></span>

<span data-ttu-id="d79fe-107">Наследуется [от apiAuthenticationConfigurationBase.](../resources/apiauthenticationconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="d79fe-107">Inherits from [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d79fe-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="d79fe-108">Properties</span></span>

|<span data-ttu-id="d79fe-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="d79fe-109">Property</span></span>|<span data-ttu-id="d79fe-110">Тип</span><span class="sxs-lookup"><span data-stu-id="d79fe-110">Type</span></span>|<span data-ttu-id="d79fe-111">Описание</span><span class="sxs-lookup"><span data-stu-id="d79fe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d79fe-112">username</span><span class="sxs-lookup"><span data-stu-id="d79fe-112">username</span></span>|<span data-ttu-id="d79fe-113">String</span><span class="sxs-lookup"><span data-stu-id="d79fe-113">String</span></span>| <span data-ttu-id="d79fe-114">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="d79fe-114">The username.</span></span> |
|<span data-ttu-id="d79fe-115">password</span><span class="sxs-lookup"><span data-stu-id="d79fe-115">password</span></span>|<span data-ttu-id="d79fe-116">Строка</span><span class="sxs-lookup"><span data-stu-id="d79fe-116">String</span></span>| <span data-ttu-id="d79fe-117">Пароль.</span><span class="sxs-lookup"><span data-stu-id="d79fe-117">The password.</span></span> <span data-ttu-id="d79fe-118">Он не возвращается в ответах.</span><span class="sxs-lookup"><span data-stu-id="d79fe-118">It is not returned in the responses.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d79fe-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="d79fe-119">Relationships</span></span>

<span data-ttu-id="d79fe-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d79fe-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d79fe-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="d79fe-121">JSON representation</span></span>

<span data-ttu-id="d79fe-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d79fe-122">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.basicAuthentication"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.basicAuthentication",
  "password": "String",
  "username": "String"
}
```
