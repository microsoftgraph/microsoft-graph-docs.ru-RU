---
title: ресурс educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: При использовании предоставления учетных данных клиента OAuth2 для подключения к поставщику данных этот тип параметров подключения следует использовать для настройки профиля.
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d38853e40d8f88bf4aa8323395848185793cc42c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500095"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="7a5d5-103">ресурс educationSynchronizationOAuth2ClientCredentialsConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="7a5d5-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

<span data-ttu-id="7a5d5-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a5d5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a5d5-105">При использовании [предоставления учетных данных клиента OAuth2](https://tools.ietf.org/html/rfc6749#section-4.4) для подключения к поставщику данных этот тип параметров подключения следует использовать для настройки профиля.</span><span class="sxs-lookup"><span data-stu-id="7a5d5-105">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="7a5d5-106">Производный от [едукатионсинчронизатионконнектионсеттингс](educationsynchronizationconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="7a5d5-106">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7a5d5-107">Свойства</span><span class="sxs-lookup"><span data-stu-id="7a5d5-107">Properties</span></span>

| <span data-ttu-id="7a5d5-108">Свойство</span><span class="sxs-lookup"><span data-stu-id="7a5d5-108">Property</span></span> | <span data-ttu-id="7a5d5-109">Тип</span><span class="sxs-lookup"><span data-stu-id="7a5d5-109">Type</span></span> | <span data-ttu-id="7a5d5-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7a5d5-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="7a5d5-111">**токенурл**</span><span class="sxs-lookup"><span data-stu-id="7a5d5-111">**tokenUrl**</span></span> | <span data-ttu-id="7a5d5-112">String</span><span class="sxs-lookup"><span data-stu-id="7a5d5-112">String</span></span> | <span data-ttu-id="7a5d5-113">URL-адрес для получения маркеров доступа для поставщика данных.</span><span class="sxs-lookup"><span data-stu-id="7a5d5-113">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="7a5d5-114">**scope**</span><span class="sxs-lookup"><span data-stu-id="7a5d5-114">**scope**</span></span> | <span data-ttu-id="7a5d5-115">String</span><span class="sxs-lookup"><span data-stu-id="7a5d5-115">String</span></span> | <span data-ttu-id="7a5d5-116">[Область запроса доступа](https://tools.ietf.org/html/rfc6749#section-3.3).</span><span class="sxs-lookup"><span data-stu-id="7a5d5-116">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7a5d5-117">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="7a5d5-117">JSON representation</span></span>
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
