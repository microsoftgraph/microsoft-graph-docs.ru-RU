---
title: тип перечисления Виндовспривацидатаакцесслевел
description: Определите категорию уровня доступа к определенной конфиденциальной информации Windows.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8ccf26f70cd76a58f2489ae1457b2c15e7c5a2d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525413"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="8e70a-103">тип перечисления Виндовспривацидатаакцесслевел</span><span class="sxs-lookup"><span data-stu-id="8e70a-103">windowsPrivacyDataAccessLevel enum type</span></span>

<span data-ttu-id="8e70a-104">Пространство имен: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8e70a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8e70a-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="8e70a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e70a-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="8e70a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e70a-107">Определите категорию уровня доступа к определенной конфиденциальной информации Windows.</span><span class="sxs-lookup"><span data-stu-id="8e70a-107">Determine the access level to specific Windows privacy data category.</span></span>

## <a name="members"></a><span data-ttu-id="8e70a-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="8e70a-108">Members</span></span>
|<span data-ttu-id="8e70a-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="8e70a-109">Member</span></span>|<span data-ttu-id="8e70a-110">Значение</span><span class="sxs-lookup"><span data-stu-id="8e70a-110">Value</span></span>|<span data-ttu-id="8e70a-111">Описание</span><span class="sxs-lookup"><span data-stu-id="8e70a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e70a-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="8e70a-112">notConfigured</span></span>|<span data-ttu-id="8e70a-113">нуль</span><span class="sxs-lookup"><span data-stu-id="8e70a-113">0</span></span>|<span data-ttu-id="8e70a-114">Уровень доступа не указан, нет целей.</span><span class="sxs-lookup"><span data-stu-id="8e70a-114">No access level specified, no intents.</span></span> <span data-ttu-id="8e70a-115">Устройство может вести себя как в Усеринконтрол, так и Форцеаллов.</span><span class="sxs-lookup"><span data-stu-id="8e70a-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="8e70a-116">Это может зависеть от данных о конфиденциальности, а также версий Windows и других факторов.</span><span class="sxs-lookup"><span data-stu-id="8e70a-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="8e70a-117">форцеаллов</span><span class="sxs-lookup"><span data-stu-id="8e70a-117">forceAllow</span></span>|<span data-ttu-id="8e70a-118">1 </span><span class="sxs-lookup"><span data-stu-id="8e70a-118">1</span></span>|<span data-ttu-id="8e70a-119">Приложениям будет разрешен доступ к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="8e70a-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="8e70a-120">форцедени</span><span class="sxs-lookup"><span data-stu-id="8e70a-120">forceDeny</span></span>|<span data-ttu-id="8e70a-121">2 </span><span class="sxs-lookup"><span data-stu-id="8e70a-121">2</span></span>|<span data-ttu-id="8e70a-122">Приложениям будет отказано в доступе к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="8e70a-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="8e70a-123">усеринконтрол</span><span class="sxs-lookup"><span data-stu-id="8e70a-123">userInControl</span></span>|<span data-ttu-id="8e70a-124">3 </span><span class="sxs-lookup"><span data-stu-id="8e70a-124">3</span></span>|<span data-ttu-id="8e70a-125">Пользователи будут получать приглашение при попытке приложения получить доступ к указанным данным о конфиденциальности.</span><span class="sxs-lookup"><span data-stu-id="8e70a-125">Users will be prompted when apps try to access specified privacy data.</span></span>|



