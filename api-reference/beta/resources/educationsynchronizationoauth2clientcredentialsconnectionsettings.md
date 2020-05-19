---
title: ресурс educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: При использовании предоставления учетных данных клиента OAuth2 для подключения к поставщику данных этот тип параметров подключения следует использовать для настройки профиля.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: dfe0a2fda8d49bd003a6ea2c23eb6a31ce619234
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289441"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="6a730-103">ресурс educationSynchronizationOAuth2ClientCredentialsConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="6a730-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

<span data-ttu-id="6a730-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a730-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a730-105">При использовании [предоставления учетных данных клиента OAuth2](https://tools.ietf.org/html/rfc6749#section-4.4) для подключения к поставщику данных этот тип параметров подключения следует использовать для настройки профиля.</span><span class="sxs-lookup"><span data-stu-id="6a730-105">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="6a730-106">Производный от [едукатионсинчронизатионконнектионсеттингс](educationsynchronizationconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="6a730-106">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="6a730-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="6a730-107">Properties</span></span>

| <span data-ttu-id="6a730-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="6a730-108">Property</span></span> | <span data-ttu-id="6a730-109">Тип</span><span class="sxs-lookup"><span data-stu-id="6a730-109">Type</span></span> | <span data-ttu-id="6a730-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6a730-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="6a730-111">**токенурл**</span><span class="sxs-lookup"><span data-stu-id="6a730-111">**tokenUrl**</span></span> | <span data-ttu-id="6a730-112">String</span><span class="sxs-lookup"><span data-stu-id="6a730-112">String</span></span> | <span data-ttu-id="6a730-113">URL-адрес для получения маркеров доступа для поставщика данных.</span><span class="sxs-lookup"><span data-stu-id="6a730-113">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="6a730-114">**scope**</span><span class="sxs-lookup"><span data-stu-id="6a730-114">**scope**</span></span> | <span data-ttu-id="6a730-115">String</span><span class="sxs-lookup"><span data-stu-id="6a730-115">String</span></span> | <span data-ttu-id="6a730-116">[Область запроса доступа](https://tools.ietf.org/html/rfc6749#section-3.3).</span><span class="sxs-lookup"><span data-stu-id="6a730-116">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6a730-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="6a730-117">JSON representation</span></span>
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
