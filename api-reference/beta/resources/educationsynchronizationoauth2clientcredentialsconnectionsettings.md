---
title: ресурс educationSynchronizationOAuth2ClientCredentialsConnectionSettings
description: При использовании предоставления учетных данных клиента OAuth2 для подключения к поставщику данных этот тип параметров подключения следует использовать для настройки профиля.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 37121868793dd76aec2c3b48182e114348d21014
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507042"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="bfbd6-103">ресурс educationSynchronizationOAuth2ClientCredentialsConnectionSettings</span><span class="sxs-lookup"><span data-stu-id="bfbd6-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bfbd6-104">При использовании [предоставления учетНых данных клиента OAuth2](https://tools.ietf.org/html/rfc6749#section-4.4) для подключения к поставщику данных этот тип параметров подключения следует использовать для настройки профиля.</span><span class="sxs-lookup"><span data-stu-id="bfbd6-104">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="bfbd6-105">Производный от [едукатионсинчронизатионконнектионсеттингс](educationsynchronizationconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="bfbd6-105">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="bfbd6-106">Свойства</span><span class="sxs-lookup"><span data-stu-id="bfbd6-106">Properties</span></span>

| <span data-ttu-id="bfbd6-107">Свойство</span><span class="sxs-lookup"><span data-stu-id="bfbd6-107">Property</span></span> | <span data-ttu-id="bfbd6-108">Тип</span><span class="sxs-lookup"><span data-stu-id="bfbd6-108">Type</span></span> | <span data-ttu-id="bfbd6-109">Описание</span><span class="sxs-lookup"><span data-stu-id="bfbd6-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="bfbd6-110">**Токенурл**</span><span class="sxs-lookup"><span data-stu-id="bfbd6-110">**tokenUrl**</span></span> | <span data-ttu-id="bfbd6-111">String</span><span class="sxs-lookup"><span data-stu-id="bfbd6-111">String</span></span> | <span data-ttu-id="bfbd6-112">URL-адрес для получения маркеров доступа для поставщика данных.</span><span class="sxs-lookup"><span data-stu-id="bfbd6-112">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="bfbd6-113">**scope**</span><span class="sxs-lookup"><span data-stu-id="bfbd6-113">**scope**</span></span> | <span data-ttu-id="bfbd6-114">String</span><span class="sxs-lookup"><span data-stu-id="bfbd6-114">String</span></span> | <span data-ttu-id="bfbd6-115">[Область запроса доступа](https://tools.ietf.org/html/rfc6749#section-3.3).</span><span class="sxs-lookup"><span data-stu-id="bfbd6-115">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bfbd6-116">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="bfbd6-116">JSON representation</span></span>
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
