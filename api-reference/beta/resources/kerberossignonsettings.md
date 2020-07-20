---
title: Тип ресурса Кербероссигнонсеттингс
description: Представляет параметры Kerberos для локального приложения, опубликованного через прокси приложения.
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0c668380c05c1a76aa971eef85f133a0e9cf8a07
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: ru-RU
ms.lasthandoff: 06/24/2020
ms.locfileid: "44862569"
---
# <a name="kerberossignonsettings-resource-type"></a><span data-ttu-id="d533e-103">Тип ресурса Кербероссигнонсеттингс</span><span class="sxs-lookup"><span data-stu-id="d533e-103">kerberosSignOnSettings resource type</span></span>

<span data-ttu-id="d533e-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d533e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d533e-105">Представляет параметры ограниченного делегирования Кеберос (ККД) для ресурса [онпремисеспублишингсинглесигнон](onpremisespublishingsinglesignon.md) при публикации локального приложения через прокси-сервер приложения Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d533e-105">Represents the Keberos Constrained Delegation (KCD) settings for the [onPremisesPublishingSingleSignOn](onpremisespublishingsinglesignon.md) resource when publishing an on-premises application via Azure AD Application Proxy.</span></span> <span data-ttu-id="d533e-106">Прокси приложения использует ограниченное делегирование Kerberos (ККД) для поддержки единого входа для встроенных приложений проверки подлинности Windows.</span><span class="sxs-lookup"><span data-stu-id="d533e-106">Application Proxy uses Kerberos Constrained Delegation (KCD) to support single-sign on to Integrated Windows Authentication applications.</span></span> <span data-ttu-id="d533e-107">Дополнительные сведения см. в статье [ограниченное делегирование Kerberos для единого входа в приложения с помощью прокси-сервера приложения](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).</span><span class="sxs-lookup"><span data-stu-id="d533e-107">For more information, see [Kerberos Constrained Delegation for single-sign on to your apps with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd).</span></span>

>[!NOTE]
><span data-ttu-id="d533e-108">Не используйте это свойство для настройки SAML или единого входа на основе пароля.</span><span class="sxs-lookup"><span data-stu-id="d533e-108">Do not use this property for configuring SAML or password-based single-sign on.</span></span> <span data-ttu-id="d533e-109">Если настраивается единый вход SAML, необходимо задать параметр [servicePrincipal](serviceprincipal.md).</span><span class="sxs-lookup"><span data-stu-id="d533e-109">If you are configuring SAML single-sign-on this must be set on the [servicePrincipal](serviceprincipal.md).</span></span>
<span data-ttu-id="d533e-110">Если вы настраиваете одиночный символ на основе пароля, его необходимо задать с помощью [креатепассвордсинглесигнонкредентиалс](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span><span class="sxs-lookup"><span data-stu-id="d533e-110">If you are configuring password-based single-sign this must be set using [createPasswordSingleSignOnCredentials](../api/serviceprincipal-createpasswordsinglesignoncredentials.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d533e-111">Свойства</span><span class="sxs-lookup"><span data-stu-id="d533e-111">Properties</span></span>

| <span data-ttu-id="d533e-112">Свойство</span><span class="sxs-lookup"><span data-stu-id="d533e-112">Property</span></span>     | <span data-ttu-id="d533e-113">Тип</span><span class="sxs-lookup"><span data-stu-id="d533e-113">Type</span></span>        | <span data-ttu-id="d533e-114">Описание</span><span class="sxs-lookup"><span data-stu-id="d533e-114">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d533e-115">кербероссервицепринЦипалнаме</span><span class="sxs-lookup"><span data-stu-id="d533e-115">kerberosServicePrincipalName</span></span>|<span data-ttu-id="d533e-116">String</span><span class="sxs-lookup"><span data-stu-id="d533e-116">String</span></span>| <span data-ttu-id="d533e-117">Внутреннее имя субъекта-службы приложения сервера приложений.</span><span class="sxs-lookup"><span data-stu-id="d533e-117">The Internal Application SPN of the application server.</span></span> <span data-ttu-id="d533e-118">Это имя участника-службы должно быть в списке служб, к которому соединитель может предоставлять делегированные учетные данные.</span><span class="sxs-lookup"><span data-stu-id="d533e-118">This SPN needs to be in the list of services to which the connector can present delegated credentials.</span></span> |
|<span data-ttu-id="d533e-119">кербероссигнонмаппингаттрибутетипе</span><span class="sxs-lookup"><span data-stu-id="d533e-119">kerberosSignOnMappingAttributeType</span></span>|<span data-ttu-id="d533e-120">String</span><span class="sxs-lookup"><span data-stu-id="d533e-120">String</span></span>| <span data-ttu-id="d533e-121">Удостоверение делегированного имени входа для соединителя, которое будет использоваться от имени ваших пользователей.</span><span class="sxs-lookup"><span data-stu-id="d533e-121">The Delegated Login Identity for the connector to use on behalf of your users.</span></span> <span data-ttu-id="d533e-122">Более подробную информацию можно узнать [в статье работа с другими локальными и облачными удостоверениями ](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities).</span><span class="sxs-lookup"><span data-stu-id="d533e-122">For more information, see [Working with different on-premises and cloud identities ](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-with-kcd#working-with-different-on-premises-and-cloud-identities).</span></span> <span data-ttu-id="d533e-123">Возможные значения: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.</span><span class="sxs-lookup"><span data-stu-id="d533e-123">Possible values are: `userPrincipalName`, `onPremisesUserPrincipalName`, `userPrincipalUsername`, `onPremisesUserPrincipalUsername`, `onPremisesSAMAccountName`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d533e-124">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="d533e-124">JSON representation</span></span>

<span data-ttu-id="d533e-125">Ниже указано представление ресурса в формате JSON.</span><span class="sxs-lookup"><span data-stu-id="d533e-125">The following is a JSON representation of the resource.</span></span>

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