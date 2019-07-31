---
title: ресурс educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: При использовании предоставления учетных данных клиента OAuth2 для подключения к поставщику данных этот тип параметров подключения следует использовать для настройки профиля.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ffc3af93a90ba0d6991007a64d24b9fb776e8bc8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972371"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="a84bd-103">ресурс educationSynchronizationOAuth2ClientCredentialsConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="a84bd-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a84bd-104">При использовании [предоставления учетных данных клиента OAuth2](https://tools.ietf.org/html/rfc6749#section-4.4) для подключения к поставщику данных этот тип параметров подключения следует использовать для настройки профиля.</span><span class="sxs-lookup"><span data-stu-id="a84bd-104">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="a84bd-105">Производный от [едукатионсинчронизатионконнектионсеттингс](educationsynchronizationconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="a84bd-105">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="a84bd-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="a84bd-106">Properties</span></span>

| <span data-ttu-id="a84bd-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="a84bd-107">Property</span></span> | <span data-ttu-id="a84bd-108">Тип</span><span class="sxs-lookup"><span data-stu-id="a84bd-108">Type</span></span> | <span data-ttu-id="a84bd-109">Описание</span><span class="sxs-lookup"><span data-stu-id="a84bd-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="a84bd-110">**Токенурл**</span><span class="sxs-lookup"><span data-stu-id="a84bd-110">**tokenUrl**</span></span> | <span data-ttu-id="a84bd-111">String</span><span class="sxs-lookup"><span data-stu-id="a84bd-111">String</span></span> | <span data-ttu-id="a84bd-112">URL-адрес для получения маркеров доступа для поставщика данных.</span><span class="sxs-lookup"><span data-stu-id="a84bd-112">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="a84bd-113">**scope**</span><span class="sxs-lookup"><span data-stu-id="a84bd-113">**scope**</span></span> | <span data-ttu-id="a84bd-114">String</span><span class="sxs-lookup"><span data-stu-id="a84bd-114">String</span></span> | <span data-ttu-id="a84bd-115">[Область запроса доступа](https://tools.ietf.org/html/rfc6749#section-3.3).</span><span class="sxs-lookup"><span data-stu-id="a84bd-115">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a84bd-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="a84bd-116">JSON representation</span></span>
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
