---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings ресурсов
description: При OAuth2 предоставить учетные данные клиента будет использоваться для подключения к поставщику данных, этот тип параметры подключения можно использовать для настройки профиля.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 37121868793dd76aec2c3b48182e114348d21014
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523556"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="268c8-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings ресурсов</span><span class="sxs-lookup"><span data-stu-id="268c8-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="268c8-104">При [OAuth2 предоставить учетные данные клиента](https://tools.ietf.org/html/rfc6749#section-4.4) будет использоваться для подключения к поставщику данных, этот тип параметры подключения можно использовать для настройки профиля.</span><span class="sxs-lookup"><span data-stu-id="268c8-104">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="268c8-105">На основе [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="268c8-105">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="268c8-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="268c8-106">Properties</span></span>

| <span data-ttu-id="268c8-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="268c8-107">Property</span></span> | <span data-ttu-id="268c8-108">Тип</span><span class="sxs-lookup"><span data-stu-id="268c8-108">Type</span></span> | <span data-ttu-id="268c8-109">Описание</span><span class="sxs-lookup"><span data-stu-id="268c8-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="268c8-110">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="268c8-110">**tokenUrl**</span></span> | <span data-ttu-id="268c8-111">String</span><span class="sxs-lookup"><span data-stu-id="268c8-111">String</span></span> | <span data-ttu-id="268c8-112">URL-адрес для получения маркера доступа для поставщика данных.</span><span class="sxs-lookup"><span data-stu-id="268c8-112">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="268c8-113">**scope**</span><span class="sxs-lookup"><span data-stu-id="268c8-113">**scope**</span></span> | <span data-ttu-id="268c8-114">String</span><span class="sxs-lookup"><span data-stu-id="268c8-114">String</span></span> | <span data-ttu-id="268c8-115">[Область запроса доступа](https://tools.ietf.org/html/rfc6749#section-3.3).</span><span class="sxs-lookup"><span data-stu-id="268c8-115">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="268c8-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="268c8-116">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationoauth2clientcredentialsconnectionsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
