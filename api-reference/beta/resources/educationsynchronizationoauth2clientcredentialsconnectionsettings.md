---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings ресурсов
description: При OAuth2 предоставить учетные данные клиента будет использоваться для подключения к поставщику данных, этот тип параметры подключения можно использовать для настройки профиля.
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 8cf7ee292b819a05a735ce6bed2a2c4fc4275907
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425458"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="e20a2-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings ресурсов</span><span class="sxs-lookup"><span data-stu-id="e20a2-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

> <span data-ttu-id="e20a2-104">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="e20a2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e20a2-105">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="e20a2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e20a2-106">При [OAuth2 предоставить учетные данные клиента](https://tools.ietf.org/html/rfc6749#section-4.4) будет использоваться для подключения к поставщику данных, этот тип параметры подключения можно использовать для настройки профиля.</span><span class="sxs-lookup"><span data-stu-id="e20a2-106">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="e20a2-107">На основе [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span><span class="sxs-lookup"><span data-stu-id="e20a2-107">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e20a2-108">Свойства</span><span class="sxs-lookup"><span data-stu-id="e20a2-108">Properties</span></span>

| <span data-ttu-id="e20a2-109">Свойство</span><span class="sxs-lookup"><span data-stu-id="e20a2-109">Property</span></span> | <span data-ttu-id="e20a2-110">Тип</span><span class="sxs-lookup"><span data-stu-id="e20a2-110">Type</span></span> | <span data-ttu-id="e20a2-111">Описание</span><span class="sxs-lookup"><span data-stu-id="e20a2-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="e20a2-112">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="e20a2-112">**tokenUrl**</span></span> | <span data-ttu-id="e20a2-113">String</span><span class="sxs-lookup"><span data-stu-id="e20a2-113">String</span></span> | <span data-ttu-id="e20a2-114">URL-адрес для получения маркера доступа для поставщика данных.</span><span class="sxs-lookup"><span data-stu-id="e20a2-114">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="e20a2-115">**scope**</span><span class="sxs-lookup"><span data-stu-id="e20a2-115">**scope**</span></span> | <span data-ttu-id="e20a2-116">String</span><span class="sxs-lookup"><span data-stu-id="e20a2-116">String</span></span> | <span data-ttu-id="e20a2-117">[Область запроса доступа](https://tools.ietf.org/html/rfc6749#section-3.3).</span><span class="sxs-lookup"><span data-stu-id="e20a2-117">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e20a2-118">Представление JSON</span><span class="sxs-lookup"><span data-stu-id="e20a2-118">JSON representation</span></span>
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
