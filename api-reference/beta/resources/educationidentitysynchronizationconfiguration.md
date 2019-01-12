---
title: Тип ресурса educationIdentitySynchronizationConfiguration
description: Абстрактный базовый класс для всех школа данных профиля identity синхронизации конфигураций. Производные классы определите поведение синхронизации удостоверения. Ниже приведены производные типы.
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 6d9841d4957d5330fc966f60a24582e101831b6c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969032"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="01899-105">Тип ресурса educationIdentitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="01899-105">educationIdentitySynchronizationConfiguration resource type</span></span>

> <span data-ttu-id="01899-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="01899-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01899-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="01899-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01899-108">Абстрактный базовый класс для всех школа данных профиля identity синхронизации конфигураций.</span><span class="sxs-lookup"><span data-stu-id="01899-108">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="01899-109">Производные классы определите поведение синхронизации удостоверения.</span><span class="sxs-lookup"><span data-stu-id="01899-109">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="01899-110">Ниже приведены производные типы.</span><span class="sxs-lookup"><span data-stu-id="01899-110">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="01899-111">Производные типы</span><span class="sxs-lookup"><span data-stu-id="01899-111">Derived types</span></span>
| <span data-ttu-id="01899-112">Тип</span><span class="sxs-lookup"><span data-stu-id="01899-112">Type</span></span> | <span data-ttu-id="01899-113">Описание</span><span class="sxs-lookup"><span data-stu-id="01899-113">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="01899-114">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="01899-114">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="01899-115">Этот тип используется в соответствии с существующим учетным записям пользователей в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="01899-115">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="01899-116">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="01899-116">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="01899-117">Этот тип используется для создания новых учетных записей пользователей в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="01899-117">Use this type to create new user accounts in Azure AD.</span></span> |
