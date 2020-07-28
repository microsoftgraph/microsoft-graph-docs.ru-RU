---
title: ресурс educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: При использовании предоставления учетных данных клиента OAuth2 для подключения к поставщику данных этот тип параметров подключения следует использовать для настройки профиля.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 00e1e531ff33f28a2e63f76925cd0b4e7759696b
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434912"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="7ff19-103">ресурс educationSynchronizationOAuth2ClientCredentialsConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="7ff19-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

<span data-ttu-id="7ff19-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ff19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ff19-105">При использовании [предоставления учетных данных клиента OAuth2](https://tools.ietf.org/html/rfc6749#section-4.4) для подключения к поставщику данных этот тип параметров подключения следует использовать для настройки профиля.</span><span class="sxs-lookup"><span data-stu-id="7ff19-105">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="7ff19-106">Производный от [едукатионсинчронизатионконнектионсеттингс].</span><span class="sxs-lookup"><span data-stu-id="7ff19-106">Derived from [educationSynchronizationConnectionSettings].</span></span>

## <a name="properties"></a><span data-ttu-id="7ff19-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7ff19-107">Properties</span></span>

| <span data-ttu-id="7ff19-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7ff19-108">Property</span></span>     | <span data-ttu-id="7ff19-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7ff19-109">Type</span></span>   | <span data-ttu-id="7ff19-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7ff19-110">Description</span></span>                                                                                                                |
| :----------- | :----- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="7ff19-111">clientId</span><span class="sxs-lookup"><span data-stu-id="7ff19-111">clientId</span></span>     | <span data-ttu-id="7ff19-112">String</span><span class="sxs-lookup"><span data-stu-id="7ff19-112">String</span></span> | <span data-ttu-id="7ff19-113">Идентификатор клиента, используемый для подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="7ff19-113">Client ID used to connect to the provider.</span></span> <span data-ttu-id="7ff19-114">Наследуется от [едукатионсинчронизатионконнектионсеттингс].</span><span class="sxs-lookup"><span data-stu-id="7ff19-114">Inherited from [educationSynchronizationConnectionSettings].</span></span>                    |
| <span data-ttu-id="7ff19-115">clientSecret</span><span class="sxs-lookup"><span data-stu-id="7ff19-115">clientSecret</span></span> | <span data-ttu-id="7ff19-116">String</span><span class="sxs-lookup"><span data-stu-id="7ff19-116">String</span></span> | <span data-ttu-id="7ff19-117">Секрет клиента для проверки подлинности подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="7ff19-117">Client secret to authenticate the connection to the provider.</span></span> <span data-ttu-id="7ff19-118">Наследуется от [едукатионсинчронизатионконнектионсеттингс].</span><span class="sxs-lookup"><span data-stu-id="7ff19-118">Inherited from [educationSynchronizationConnectionSettings].</span></span> |
| <span data-ttu-id="7ff19-119">токенурл</span><span class="sxs-lookup"><span data-stu-id="7ff19-119">tokenUrl</span></span>     | <span data-ttu-id="7ff19-120">Строка</span><span class="sxs-lookup"><span data-stu-id="7ff19-120">String</span></span> | <span data-ttu-id="7ff19-121">URL-адрес для получения маркеров доступа для поставщика данных.</span><span class="sxs-lookup"><span data-stu-id="7ff19-121">The URL to get access tokens for the data provider.</span></span>                                                                        |
| <span data-ttu-id="7ff19-122">scope</span><span class="sxs-lookup"><span data-stu-id="7ff19-122">scope</span></span>        | <span data-ttu-id="7ff19-123">Строка</span><span class="sxs-lookup"><span data-stu-id="7ff19-123">String</span></span> | <span data-ttu-id="7ff19-124">Область запроса доступа (см. [RFC6749](https://tools.ietf.org/html/rfc6749#section-3.3)).</span><span class="sxs-lookup"><span data-stu-id="7ff19-124">The scope of the access request (see [RFC6749](https://tools.ietf.org/html/rfc6749#section-3.3)).</span></span>                          |

[едукатионсинчронизатионконнектионсеттингс]: educationsynchronizationconnectionsettings.md
[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md

## <a name="json-representation"></a><span data-ttu-id="7ff19-126">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7ff19-126">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
}-->

```json
{
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings",
  "clientId": "String",
  "clientSecret": "String",
  "tokenUrl": "String",
  "scope": "String"
}
```
