---
title: Тип ресурса Едукатионсинчронизатионконнектионсеттингс
description: 'Представляет параметры подключения к поставщику. Это позволяет системе узнать, как подключаться к API поставщика. '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 387c002240d54d1ec12e58564e91831d6f0e8a50
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334121"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="b3b15-104">Тип ресурса Едукатионсинчронизатионконнектионсеттингс</span><span class="sxs-lookup"><span data-stu-id="b3b15-104">educationSynchronizationConnectionSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3b15-105">Представляет параметры подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="b3b15-105">Represents the provider connection settings.</span></span> <span data-ttu-id="b3b15-106">Это позволяет системе узнать, как подключаться к API поставщика.</span><span class="sxs-lookup"><span data-stu-id="b3b15-106">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="b3b15-107">**Примечание:** Этот сложный тип является абстрактным.</span><span class="sxs-lookup"><span data-stu-id="b3b15-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="b3b15-108">Ознакомьтесь со списками определенных типов параметров подключения.</span><span class="sxs-lookup"><span data-stu-id="b3b15-108">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="b3b15-109">ПроизВодные типы</span><span class="sxs-lookup"><span data-stu-id="b3b15-109">Derived types</span></span>
| <span data-ttu-id="b3b15-110">Тип</span><span class="sxs-lookup"><span data-stu-id="b3b15-110">Type</span></span> | <span data-ttu-id="b3b15-111">Описание</span><span class="sxs-lookup"><span data-stu-id="b3b15-111">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="b3b15-112">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="b3b15-112">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="b3b15-113">Используйте этот тип для предоставления параметров подключения OAuth1.</span><span class="sxs-lookup"><span data-stu-id="b3b15-113">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="b3b15-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="b3b15-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="b3b15-115">Используйте этот тип для предоставления учетных данных клиента OAuth2 для предоставления параметров подключения.</span><span class="sxs-lookup"><span data-stu-id="b3b15-115">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="b3b15-116">Свойства</span><span class="sxs-lookup"><span data-stu-id="b3b15-116">Properties</span></span>

| <span data-ttu-id="b3b15-117">Свойство</span><span class="sxs-lookup"><span data-stu-id="b3b15-117">Property</span></span> | <span data-ttu-id="b3b15-118">Тип</span><span class="sxs-lookup"><span data-stu-id="b3b15-118">Type</span></span> | <span data-ttu-id="b3b15-119">Описание</span><span class="sxs-lookup"><span data-stu-id="b3b15-119">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="b3b15-120">**clientId**</span><span class="sxs-lookup"><span data-stu-id="b3b15-120">**clientId**</span></span> | <span data-ttu-id="b3b15-121">String</span><span class="sxs-lookup"><span data-stu-id="b3b15-121">String</span></span> |  <span data-ttu-id="b3b15-122">Идентификатор клиента, используемый для подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="b3b15-122">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="b3b15-123">**clientSecret**</span><span class="sxs-lookup"><span data-stu-id="b3b15-123">**clientSecret**</span></span> | <span data-ttu-id="b3b15-124">String</span><span class="sxs-lookup"><span data-stu-id="b3b15-124">String</span></span> |  <span data-ttu-id="b3b15-125">Секрет клиента для проверки подлинности подключения к поставщику.</span><span class="sxs-lookup"><span data-stu-id="b3b15-125">Client secret to authenticate the connection to the provider.</span></span> |
