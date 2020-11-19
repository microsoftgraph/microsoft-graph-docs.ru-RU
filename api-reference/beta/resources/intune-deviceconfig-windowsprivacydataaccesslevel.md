---
title: тип перечисления Виндовспривацидатаакцесслевел
description: Определите категорию уровня доступа к определенной конфиденциальной информации Windows.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: acd71682d7e682dec53bb87885374aabdd38089d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49215193"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="07511-103">тип перечисления Виндовспривацидатаакцесслевел</span><span class="sxs-lookup"><span data-stu-id="07511-103">windowsPrivacyDataAccessLevel enum type</span></span>

<span data-ttu-id="07511-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07511-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07511-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="07511-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07511-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="07511-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07511-107">Определите категорию уровня доступа к определенной конфиденциальной информации Windows.</span><span class="sxs-lookup"><span data-stu-id="07511-107">Determine the access level to specific Windows privacy data category.</span></span>

## <a name="members"></a><span data-ttu-id="07511-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="07511-108">Members</span></span>
|<span data-ttu-id="07511-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="07511-109">Member</span></span>|<span data-ttu-id="07511-110">Значение</span><span class="sxs-lookup"><span data-stu-id="07511-110">Value</span></span>|<span data-ttu-id="07511-111">Описание</span><span class="sxs-lookup"><span data-stu-id="07511-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07511-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="07511-112">notConfigured</span></span>|<span data-ttu-id="07511-113">нуль</span><span class="sxs-lookup"><span data-stu-id="07511-113">0</span></span>|<span data-ttu-id="07511-114">Уровень доступа не указан, нет целей.</span><span class="sxs-lookup"><span data-stu-id="07511-114">No access level specified, no intents.</span></span> <span data-ttu-id="07511-115">Устройство может вести себя как в Усеринконтрол, так и Форцеаллов.</span><span class="sxs-lookup"><span data-stu-id="07511-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="07511-116">Это может зависеть от данных о конфиденциальности, а также версий Windows и других факторов.</span><span class="sxs-lookup"><span data-stu-id="07511-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="07511-117">форцеаллов</span><span class="sxs-lookup"><span data-stu-id="07511-117">forceAllow</span></span>|<span data-ttu-id="07511-118">1,1</span><span class="sxs-lookup"><span data-stu-id="07511-118">1</span></span>|<span data-ttu-id="07511-119">Приложениям будет разрешен доступ к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="07511-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="07511-120">форцедени</span><span class="sxs-lookup"><span data-stu-id="07511-120">forceDeny</span></span>|<span data-ttu-id="07511-121">2</span><span class="sxs-lookup"><span data-stu-id="07511-121">2</span></span>|<span data-ttu-id="07511-122">Приложениям будет отказано в доступе к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="07511-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="07511-123">усеринконтрол</span><span class="sxs-lookup"><span data-stu-id="07511-123">userInControl</span></span>|<span data-ttu-id="07511-124">4</span><span class="sxs-lookup"><span data-stu-id="07511-124">3</span></span>|<span data-ttu-id="07511-125">Пользователи будут получать приглашение при попытке приложения получить доступ к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="07511-125">Users will be prompted when apps try to access specified privacy data.</span></span>|




