---
title: Тип ресурса Едукатионсинчронизатионконнектионсеттингс
description: 'Представляет параметры подключения к поставщику. Это позволяет системе узнать, как подключаться к API поставщика. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9d972aec91218dfc9606da4c8aa88e27b63167d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500571"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="2708b-104">Тип ресурса Едукатионсинчронизатионконнектионсеттингс</span><span class="sxs-lookup"><span data-stu-id="2708b-104">educationSynchronizationConnectionSettings resource type</span></span>

<span data-ttu-id="2708b-105">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2708b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2708b-106">Представляет параметры подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="2708b-106">Represents the provider connection settings.</span></span> <span data-ttu-id="2708b-107">Это позволяет системе узнать, как подключаться к API поставщика.</span><span class="sxs-lookup"><span data-stu-id="2708b-107">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="2708b-108">**Примечание:** Этот сложный тип является абстрактным.</span><span class="sxs-lookup"><span data-stu-id="2708b-108">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="2708b-109">Ознакомьтесь со списками определенных типов параметров подключения.</span><span class="sxs-lookup"><span data-stu-id="2708b-109">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="2708b-110">Производные типы</span><span class="sxs-lookup"><span data-stu-id="2708b-110">Derived types</span></span>
| <span data-ttu-id="2708b-111">Тип</span><span class="sxs-lookup"><span data-stu-id="2708b-111">Type</span></span> | <span data-ttu-id="2708b-112">Описание</span><span class="sxs-lookup"><span data-stu-id="2708b-112">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="2708b-113">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="2708b-113">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="2708b-114">Используйте этот тип для предоставления параметров подключения OAuth1.</span><span class="sxs-lookup"><span data-stu-id="2708b-114">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="2708b-115">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="2708b-115">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="2708b-116">Используйте этот тип для предоставления учетных данных клиента OAuth2 для предоставления параметров подключения.</span><span class="sxs-lookup"><span data-stu-id="2708b-116">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="2708b-117">Свойства</span><span class="sxs-lookup"><span data-stu-id="2708b-117">Properties</span></span>

| <span data-ttu-id="2708b-118">Свойство</span><span class="sxs-lookup"><span data-stu-id="2708b-118">Property</span></span> | <span data-ttu-id="2708b-119">Тип</span><span class="sxs-lookup"><span data-stu-id="2708b-119">Type</span></span> | <span data-ttu-id="2708b-120">Описание</span><span class="sxs-lookup"><span data-stu-id="2708b-120">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="2708b-121">**clientId**</span><span class="sxs-lookup"><span data-stu-id="2708b-121">**clientId**</span></span> | <span data-ttu-id="2708b-122">String</span><span class="sxs-lookup"><span data-stu-id="2708b-122">String</span></span> |  <span data-ttu-id="2708b-123">Идентификатор клиента, используемый для подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="2708b-123">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="2708b-124">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="2708b-124">**clientSecret**</span></span> | <span data-ttu-id="2708b-125">String</span><span class="sxs-lookup"><span data-stu-id="2708b-125">String</span></span> |  <span data-ttu-id="2708b-126">Секрет клиента для проверки подлинности подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="2708b-126">Client secret to authenticate the connection to the provider.</span></span> |
