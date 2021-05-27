---
title: тип ресурса authenticationMethodsRegistrationCampaign
description: Представляет параметры, используемые для запуска кампаний, чтобы подтолкнуть пользователей к настройке целевых методов проверки подлинности.
author: mjsantani
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: be989bc86e5e708a89cd33c700e57edce42d9e50
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682935"
---
# <a name="authenticationmethodsregistrationcampaign-resource-type"></a><span data-ttu-id="1b467-103">тип ресурса authenticationMethodsRegistrationCampaign</span><span class="sxs-lookup"><span data-stu-id="1b467-103">authenticationMethodsRegistrationCampaign resource type</span></span>

<span data-ttu-id="1b467-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1b467-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1b467-105">Представляет параметры, используемые для запуска кампаний, чтобы подтолкнуть пользователей к настройке целевых методов проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="1b467-105">Represents the settings used to run campaigns to push users to set up targeted authentication methods.</span></span> <span data-ttu-id="1b467-106">Пользователям предложено настроить метод проверки подлинности после успешного выполнения задачи MFA.</span><span class="sxs-lookup"><span data-stu-id="1b467-106">Users are prompted to set up the authentication method after they successfully complete a MFA challenge.</span></span> <span data-ttu-id="1b467-107">Доступно только для приложения Microsoft Authenticator для MFA.</span><span class="sxs-lookup"><span data-stu-id="1b467-107">Only available for the Microsoft Authenticator app for MFA.</span></span>

## <a name="properties"></a><span data-ttu-id="1b467-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="1b467-108">Properties</span></span>
|<span data-ttu-id="1b467-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="1b467-109">Property</span></span>|<span data-ttu-id="1b467-110">Тип</span><span class="sxs-lookup"><span data-stu-id="1b467-110">Type</span></span>|<span data-ttu-id="1b467-111">Описание</span><span class="sxs-lookup"><span data-stu-id="1b467-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b467-112">excludeTargets</span><span class="sxs-lookup"><span data-stu-id="1b467-112">excludeTargets</span></span>|<span data-ttu-id="1b467-113">[excludeTarget](../resources/excludetarget.md) collection</span><span class="sxs-lookup"><span data-stu-id="1b467-113">[excludeTarget](../resources/excludetarget.md) collection</span></span>|<span data-ttu-id="1b467-114">Пользователям и группам пользователей, которые не могут быть предложены к настройкам метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="1b467-114">Users and groups of users that are excluded from being prompted to set up the authentication method.</span></span>|
|<span data-ttu-id="1b467-115">includeTargets</span><span class="sxs-lookup"><span data-stu-id="1b467-115">includeTargets</span></span>|<span data-ttu-id="1b467-116">[authenticationMethodsRegistrationCampaignIncludeTarget](../resources/authenticationmethodsregistrationcampaignincludetarget.md) collection</span><span class="sxs-lookup"><span data-stu-id="1b467-116">[authenticationMethodsRegistrationCampaignIncludeTarget](../resources/authenticationmethodsregistrationcampaignincludetarget.md) collection</span></span>|<span data-ttu-id="1b467-117">Пользователи и группы пользователей, которые могут настроить метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="1b467-117">Users and groups of users that are prompted to set up the authentication method.</span></span>|
|<span data-ttu-id="1b467-118">snoozeDurationInDays</span><span class="sxs-lookup"><span data-stu-id="1b467-118">snoozeDurationInDays</span></span>|<span data-ttu-id="1b467-119">Int32</span><span class="sxs-lookup"><span data-stu-id="1b467-119">Int32</span></span>|<span data-ttu-id="1b467-120">Указывает количество дней, когда пользователь снова видит подсказку, если он выбирает "Не сейчас" и не видит запрос.</span><span class="sxs-lookup"><span data-stu-id="1b467-120">Specifies the number of days that the user sees a prompt again if they select "Not now" and snoozes the prompt.</span></span> <span data-ttu-id="1b467-121">Минимум 0 дней.</span><span class="sxs-lookup"><span data-stu-id="1b467-121">Minimum 0 days.</span></span> <span data-ttu-id="1b467-122">Максимум: 14 дней.</span><span class="sxs-lookup"><span data-stu-id="1b467-122">Maximum: 14 days.</span></span> <span data-ttu-id="1b467-123">Если значение "0" — пользователь получает запрос во время каждой попытки MFA.</span><span class="sxs-lookup"><span data-stu-id="1b467-123">If the value is “0” – The user is prompted during every MFA attempt.</span></span>|
|<span data-ttu-id="1b467-124">state</span><span class="sxs-lookup"><span data-stu-id="1b467-124">state</span></span>|<span data-ttu-id="1b467-125">advancedConfigState</span><span class="sxs-lookup"><span data-stu-id="1b467-125">advancedConfigState</span></span>|<span data-ttu-id="1b467-126">Включить или отключить функцию.</span><span class="sxs-lookup"><span data-stu-id="1b467-126">Enable or disable the feature.</span></span> <span data-ttu-id="1b467-127">Возможные значения: `default`, `enabled`, `disabled`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="1b467-127">Possible values are: `default`, `enabled`, `disabled`, `unknownFutureValue`.</span></span> <span data-ttu-id="1b467-128">Значение используется, когда конфигурация не была явно заданная и использует для параметра поведение `default` Azure AD по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="1b467-128">The `default` value is used when the configuration hasn't been explicitly set and uses the default behavior of Azure AD for the setting.</span></span> <span data-ttu-id="1b467-129">Значение по умолчанию — `disabled`.</span><span class="sxs-lookup"><span data-stu-id="1b467-129">The default value is `disabled`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b467-130">Связи</span><span class="sxs-lookup"><span data-stu-id="1b467-130">Relationships</span></span>
<span data-ttu-id="1b467-131">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="1b467-131">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b467-132">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="1b467-132">JSON representation</span></span>
<span data-ttu-id="1b467-133">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="1b467-133">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaign"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.authenticationMethodsRegistrationCampaign",
  "excludeTargets": [
    {
      "@odata.type": "microsoft.graph.excludeTarget"
    }
  ],
  "includeTargets": [
    {
      "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaignIncludeTarget"
    }
  ],
  "snoozeDurationInDays": "Integer",
  "state": "String"
}
```
