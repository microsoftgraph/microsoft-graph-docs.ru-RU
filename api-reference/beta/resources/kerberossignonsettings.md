---
title: тип ресурса kerberosSignOnSettings
description: Представляет параметры kerberos для локального приложения, опубликованного через Application Proxy.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: af00e70e1ef4603c1b1370ec5ef9e9ba75fecb4c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943665"
---
# <a name="kerberossignonsettings-resource-type"></a><span data-ttu-id="6b384-103">тип ресурса kerberosSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="6b384-103">kerberosSignOnSettings resource type</span></span>

<span data-ttu-id="6b384-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b384-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6b384-105">Представляет параметры ограниченной делегирования Keberos (KCD) для ресурса [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) при публикации локального приложения с помощью прокси-сервера приложения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="6b384-105">Represents the Keberos Constrained Delegation (KCD) settings for the [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) resource when publishing an on-premises application via Azure AD Application Proxy.</span></span> <span data-ttu-id="6b384-106">Прокси-сервер приложения использует ограниченное делегирование Kerberos (KCD) для поддержки однорегистрирования в интегрированных приложениях проверки подлинности Windows.</span><span class="sxs-lookup"><span data-stu-id="6b384-106">Application Proxy uses Kerberos Constrained Delegation (KCD) to support single-sign on to Integrated Windows Authentication applications.</span></span> <span data-ttu-id="6b384-107">Дополнительные сведения см. в документе [Kerberos Constrained Delegation for single-sign on to your apps with Application Proxy.](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd)</span><span class="sxs-lookup"><span data-stu-id="6b384-107">For more information, see [Kerberos Constrained Delegation for single-sign on to your apps with Application Proxy](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).</span></span>

>[!NOTE]
><span data-ttu-id="6b384-108">Не используйте это свойство для настройки единого знака SAML или пароля.</span><span class="sxs-lookup"><span data-stu-id="6b384-108">Do not use this property for configuring SAML or password-based single-sign on.</span></span> <span data-ttu-id="6b384-109">Если вы настраивает SAML с одним входом, это должно быть установлено на [службеPrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="6b384-109">If you are configuring SAML single-sign-on this must be set on the [servicePrincipal](serviceprincipal.md).</span></span>
<span data-ttu-id="6b384-110">Если вы настраивает однонаправленный пароль, это необходимо установить с помощью [createPasswordSingleSignOnCredentials.](../api/serviceprincipal-createpasswordsinglesignoncredentials.md)</span><span class="sxs-lookup"><span data-stu-id="6b384-110">If you are configuring password-based single-sign this must be set using [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6b384-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="6b384-111">Properties</span></span>

| <span data-ttu-id="6b384-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="6b384-112">Property</span></span>     | <span data-ttu-id="6b384-113">Тип</span><span class="sxs-lookup"><span data-stu-id="6b384-113">Type</span></span>        | <span data-ttu-id="6b384-114">Описание</span><span class="sxs-lookup"><span data-stu-id="6b384-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="6b384-115">kerberosServicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="6b384-115">kerberosServicePrincipalName</span></span>|<span data-ttu-id="6b384-116">Строка</span><span class="sxs-lookup"><span data-stu-id="6b384-116">String</span></span>| <span data-ttu-id="6b384-117">SpN внутреннего приложения сервера приложений.</span><span class="sxs-lookup"><span data-stu-id="6b384-117">The Internal Application SPN of the application server.</span></span> <span data-ttu-id="6b384-118">Этот SPN должен быть в списке служб, которым соединитатель может представлять делегированную учетную данные.</span><span class="sxs-lookup"><span data-stu-id="6b384-118">This SPN needs to be in the list of services to which the connector can present delegated credentials.</span></span> |
|<span data-ttu-id="6b384-119">kerberosSignOnMappingAttributeType</span><span class="sxs-lookup"><span data-stu-id="6b384-119">kerberosSignOnMappingAttributeType</span></span>|<span data-ttu-id="6b384-120">kerberosSignOnMappingAttributeType</span><span class="sxs-lookup"><span data-stu-id="6b384-120">kerberosSignOnMappingAttributeType</span></span>| <span data-ttu-id="6b384-121">Удостоверение делегирования входа, используемое соединитетелем от имени пользователей.</span><span class="sxs-lookup"><span data-stu-id="6b384-121">The Delegated Login Identity for the connector to use on behalf of your users.</span></span> <span data-ttu-id="6b384-122">Дополнительные сведения см. в ссылке Работа с различными [локальной и облачной идентификаторами. ](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities)</span><span class="sxs-lookup"><span data-stu-id="6b384-122">For more information, see [Working with different on-premises and cloud identities ](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities).</span></span> <span data-ttu-id="6b384-123">Возможные значения: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.</span><span class="sxs-lookup"><span data-stu-id="6b384-123">Possible values are: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b384-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6b384-124">JSON representation</span></span>

<span data-ttu-id="6b384-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="6b384-125">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.kerberosSignOnSettings",
  "baseType": null
}-->

```json
{
  "kerberosServicePrincipalName": "String",
  "kerberosSignOnMappingAttributeType": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "kerberosSignOnSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
