---
title: Тип ресурса educationIdentitySynchronizationConfiguration
description: Абстрактный базовый класс для всех школа данных профиля identity синхронизации конфигураций. Производные классы определите поведение синхронизации удостоверения. Ниже приведены производные типы.
author: mmast-msft
ms.openlocfilehash: d32eb2b06cb76c578edf4a80e73e5bf6ec6b4757
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334456"
---
# <a name="educationidentitysynchronizationconfiguration-resource-type"></a><span data-ttu-id="43128-105">Тип ресурса educationIdentitySynchronizationConfiguration</span><span class="sxs-lookup"><span data-stu-id="43128-105">educationIdentitySynchronizationConfiguration resource type</span></span>

> <span data-ttu-id="43128-106">**Важно!** API бета-версии (/beta) в Microsoft Graph проходят тестирование и могут быть изменены.</span><span class="sxs-lookup"><span data-stu-id="43128-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="43128-107">Использование этих API в производственных приложениях не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="43128-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="43128-108">Абстрактный базовый класс для всех школа данных профиля identity синхронизации конфигураций.</span><span class="sxs-lookup"><span data-stu-id="43128-108">Abstract base class for all school data profile identity synchronization configurations.</span></span> <span data-ttu-id="43128-109">Производные классы определите поведение синхронизации удостоверения.</span><span class="sxs-lookup"><span data-stu-id="43128-109">The derived classes define the behavior for synchronizing identities.</span></span> <span data-ttu-id="43128-110">Ниже приведены производные типы.</span><span class="sxs-lookup"><span data-stu-id="43128-110">The following are the derived types.</span></span>

## <a name="derived-types"></a><span data-ttu-id="43128-111">Производные типы</span><span class="sxs-lookup"><span data-stu-id="43128-111">Derived types</span></span>
| <span data-ttu-id="43128-112">Тип</span><span class="sxs-lookup"><span data-stu-id="43128-112">Type</span></span> | <span data-ttu-id="43128-113">Описание</span><span class="sxs-lookup"><span data-stu-id="43128-113">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="43128-114">**educationIdentityMatchingConfiguration**</span><span class="sxs-lookup"><span data-stu-id="43128-114">**educationIdentityMatchingConfiguration**</span></span>](educationidentitymatchingconfiguration.md) | <span data-ttu-id="43128-115">Этот тип используется в соответствии с существующим учетным записям пользователей в Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="43128-115">Use this type to match existing user accounts in Azure Active Directory (Azure AD).</span></span> |
| [<span data-ttu-id="43128-116">**educationIdentityCreationConfiguration**</span><span class="sxs-lookup"><span data-stu-id="43128-116">**educationIdentityCreationConfiguration**</span></span>](educationidentitycreationconfiguration.md) | <span data-ttu-id="43128-117">Этот тип используется для создания новых учетных записей пользователей в Azure AD.</span><span class="sxs-lookup"><span data-stu-id="43128-117">Use this type to create new user accounts in Azure AD.</span></span> |
