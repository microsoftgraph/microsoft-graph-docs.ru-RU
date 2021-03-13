---
title: тип ресурса basicAuthentication
description: Представляет конфигурацию для использования базовой проверки подлинности в вызове API.
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 396cadec8e1766bee662c51df8d7999ba6a0ba6c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761690"
---
# <a name="basicauthentication-resource-type"></a><span data-ttu-id="10327-103">тип ресурса basicAuthentication</span><span class="sxs-lookup"><span data-stu-id="10327-103">basicAuthentication resource type</span></span>

<span data-ttu-id="10327-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="10327-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="10327-105">Представляет конфигурацию для использования проверки подлинности HTTP Basic, которая влечет за собой имя пользователя и пароль, в вызове API.</span><span class="sxs-lookup"><span data-stu-id="10327-105">Represents configuration for using HTTP Basic authentication, which entails a username and password, in an API call.</span></span> <span data-ttu-id="10327-106">Имя пользователя и пароль отправляются в качестве загона авторизации в качестве базовой версии 64 кодированной версии `Basic {value}` `value` username:password.</span><span class="sxs-lookup"><span data-stu-id="10327-106">The username and password is sent as the Authorization header as `Basic {value}` where `value` is base 64 encoded version of username:password.</span></span>

<span data-ttu-id="10327-107">Наследует [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span><span class="sxs-lookup"><span data-stu-id="10327-107">Inherits from [apiAuthenticationConfigurationBase](../resources/apiauthenticationconfigurationbase.md).</span></span>

## <a name="properties"></a><span data-ttu-id="10327-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="10327-108">Properties</span></span>

|<span data-ttu-id="10327-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="10327-109">Property</span></span>|<span data-ttu-id="10327-110">Тип</span><span class="sxs-lookup"><span data-stu-id="10327-110">Type</span></span>|<span data-ttu-id="10327-111">Описание</span><span class="sxs-lookup"><span data-stu-id="10327-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10327-112">username</span><span class="sxs-lookup"><span data-stu-id="10327-112">username</span></span>|<span data-ttu-id="10327-113">String</span><span class="sxs-lookup"><span data-stu-id="10327-113">String</span></span>| <span data-ttu-id="10327-114">Имя пользователя.</span><span class="sxs-lookup"><span data-stu-id="10327-114">The username.</span></span> |
|<span data-ttu-id="10327-115">password</span><span class="sxs-lookup"><span data-stu-id="10327-115">password</span></span>|<span data-ttu-id="10327-116">Строка</span><span class="sxs-lookup"><span data-stu-id="10327-116">String</span></span>| <span data-ttu-id="10327-117">Пароль.</span><span class="sxs-lookup"><span data-stu-id="10327-117">The password.</span></span> <span data-ttu-id="10327-118">Он не возвращается в ответах.</span><span class="sxs-lookup"><span data-stu-id="10327-118">It is not returned in the responses.</span></span> |

## <a name="relationships"></a><span data-ttu-id="10327-119">Отношения</span><span class="sxs-lookup"><span data-stu-id="10327-119">Relationships</span></span>

<span data-ttu-id="10327-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="10327-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="10327-121">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="10327-121">JSON representation</span></span>

<span data-ttu-id="10327-122">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="10327-122">The following is a JSON representation of the resource.</span></span>
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
