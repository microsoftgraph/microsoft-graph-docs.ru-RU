---
title: тип ресурса registrationEnforcement
description: Принудительное выполнение регистрации во время регистрации.
author: mjsantani
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 86d3e974ccfebdf0011c9c19f881096e3fb2ba40
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682918"
---
# <a name="registrationenforcement-resource-type"></a><span data-ttu-id="c46de-103">тип ресурса registrationEnforcement</span><span class="sxs-lookup"><span data-stu-id="c46de-103">registrationEnforcement resource type</span></span>

<span data-ttu-id="c46de-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c46de-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c46de-105">Принудительное выполнение регистрации во время регистрации.</span><span class="sxs-lookup"><span data-stu-id="c46de-105">Enforce registration at sign-in time.</span></span> <span data-ttu-id="c46de-106">В настоящее время это может использоваться только для напоминания пользователям о том, как настроить целевые методы проверки подлинности (Microsoft Authenticator) с помощью "authenticationMethodsRegistrationCampaign".</span><span class="sxs-lookup"><span data-stu-id="c46de-106">This can currently only be used to remind users to set up targeted authentication methods (Microsoft Authenticator) using the 'authenticationMethodsRegistrationCampaign\`.</span></span>

## <a name="properties"></a><span data-ttu-id="c46de-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="c46de-107">Properties</span></span>
|<span data-ttu-id="c46de-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="c46de-108">Property</span></span>|<span data-ttu-id="c46de-109">Тип</span><span class="sxs-lookup"><span data-stu-id="c46de-109">Type</span></span>|<span data-ttu-id="c46de-110">Описание</span><span class="sxs-lookup"><span data-stu-id="c46de-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c46de-111">authenticationMethodsRegistrationCampaign</span><span class="sxs-lookup"><span data-stu-id="c46de-111">authenticationMethodsRegistrationCampaign</span></span>|[<span data-ttu-id="c46de-112">authenticationMethodsRegistrationCampaign</span><span class="sxs-lookup"><span data-stu-id="c46de-112">authenticationMethodsRegistrationCampaign</span></span>](../resources/authenticationmethodsregistrationcampaign.md)|<span data-ttu-id="c46de-113">Запустите кампании, чтобы напомнить пользователям о настройке целевых методов проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="c46de-113">Run campaigns to remind users to setup targeted authentication methods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c46de-114">Связи</span><span class="sxs-lookup"><span data-stu-id="c46de-114">Relationships</span></span>
<span data-ttu-id="c46de-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c46de-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c46de-116">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="c46de-116">JSON representation</span></span>
<span data-ttu-id="c46de-117">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="c46de-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.registrationEnforcement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.registrationEnforcement",
  "authenticationMethodsRegistrationCampaign": {
    "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaign"
  }
}
```
