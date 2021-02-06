---
title: Тип ресурса kerberosSignOnSettings
description: Представляет параметры kerberos для локального приложения, опубликованного через прокси приложения.
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: resourcePageType
ms.openlocfilehash: 0220d6d85c7aafe3489e4099a2c6b1837a7439e2
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130089"
---
# <a name="kerberossignonsettings-resource-type"></a><span data-ttu-id="86018-103">Тип ресурса kerberosSignOnSettings</span><span class="sxs-lookup"><span data-stu-id="86018-103">kerberosSignOnSettings resource type</span></span>

<span data-ttu-id="86018-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86018-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="86018-105">Представляет параметры ограниченного делегирования Keberos (KCD) для ресурса [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) при публикации локального приложения через прокси приложения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="86018-105">Represents the Keberos Constrained Delegation (KCD) settings for the [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) resource when publishing an on-premises application via Azure AD Application Proxy.</span></span> <span data-ttu-id="86018-106">Прокси приложения использует ограниченное делегирование Kerberos (KCD) для поддержки единого вход в интегрированные приложения проверки подлинности Windows.</span><span class="sxs-lookup"><span data-stu-id="86018-106">Application Proxy uses Kerberos Constrained Delegation (KCD) to support single-sign on to Integrated Windows Authentication applications.</span></span> <span data-ttu-id="86018-107">Дополнительные сведения см. в сведениях о ограниченном делегирования [Kerberos](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd)для единого вход в приложения с помощью прокси приложения.</span><span class="sxs-lookup"><span data-stu-id="86018-107">For more information, see [Kerberos Constrained Delegation for single-sign on to your apps with Application Proxy](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).</span></span>

>[!NOTE]
><span data-ttu-id="86018-108">Не используйте это свойство для настройки samL или единого вход на основе пароля.</span><span class="sxs-lookup"><span data-stu-id="86018-108">Do not use this property for configuring SAML or password-based single-sign on.</span></span> <span data-ttu-id="86018-109">Если вы настраиваете единый вход SAML, это должно быть установлено в [servicePrincipal.](serviceprincipal.md)</span><span class="sxs-lookup"><span data-stu-id="86018-109">If you are configuring SAML single-sign-on this must be set on the [servicePrincipal](serviceprincipal.md).</span></span>
<span data-ttu-id="86018-110">При настройке единого знака на основе пароля этот код необходимо настроить с помощью [createPasswordSingleSignOnCredentials.](../api/serviceprincipal-createpasswordsinglesignoncredentials.md)</span><span class="sxs-lookup"><span data-stu-id="86018-110">If you are configuring password-based single-sign this must be set using [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span></span>

## <a name="properties"></a><span data-ttu-id="86018-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="86018-111">Properties</span></span>

| <span data-ttu-id="86018-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="86018-112">Property</span></span>     | <span data-ttu-id="86018-113">Тип</span><span class="sxs-lookup"><span data-stu-id="86018-113">Type</span></span>        | <span data-ttu-id="86018-114">Описание</span><span class="sxs-lookup"><span data-stu-id="86018-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="86018-115">kerberosServicePrincipalName</span><span class="sxs-lookup"><span data-stu-id="86018-115">kerberosServicePrincipalName</span></span>|<span data-ttu-id="86018-116">Строка</span><span class="sxs-lookup"><span data-stu-id="86018-116">String</span></span>| <span data-ttu-id="86018-117">Внутреннее spN приложения сервера приложений.</span><span class="sxs-lookup"><span data-stu-id="86018-117">The Internal Application SPN of the application server.</span></span> <span data-ttu-id="86018-118">Это SPN должно быть в списке служб, которым соединители могут представлять делегированную учетную данные.</span><span class="sxs-lookup"><span data-stu-id="86018-118">This SPN needs to be in the list of services to which the connector can present delegated credentials.</span></span> |
|<span data-ttu-id="86018-119">kerberosSignOnMappingAttributeType</span><span class="sxs-lookup"><span data-stu-id="86018-119">kerberosSignOnMappingAttributeType</span></span>|<span data-ttu-id="86018-120">Строка</span><span class="sxs-lookup"><span data-stu-id="86018-120">String</span></span>| <span data-ttu-id="86018-121">Делегированная идентификация для входа в систему, используемая соединитетелем от имени пользователей.</span><span class="sxs-lookup"><span data-stu-id="86018-121">The Delegated Login Identity for the connector to use on behalf of your users.</span></span> <span data-ttu-id="86018-122">Дополнительные сведения см. в работе с различными идентификаторами локальной и [облачной платформы. ](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities)</span><span class="sxs-lookup"><span data-stu-id="86018-122">For more information, see [Working with different on-premises and cloud identities ](/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities).</span></span> <span data-ttu-id="86018-123">Возможные значения: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.</span><span class="sxs-lookup"><span data-stu-id="86018-123">Possible values are: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86018-124">Представление в формате JSON</span><span class="sxs-lookup"><span data-stu-id="86018-124">JSON representation</span></span>

<span data-ttu-id="86018-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="86018-125">The following is a JSON representation of the resource.</span></span>

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
