---
title: тип перечисления Виндовссмодеконфигуратион
description: Возможные варианты настройки S режима разблокировки
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ff0a38f51f4ff4e33d2f6df4e8955c34b34192de
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49231341"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="0c899-103">тип перечисления Виндовссмодеконфигуратион</span><span class="sxs-lookup"><span data-stu-id="0c899-103">windowsSModeConfiguration enum type</span></span>

<span data-ttu-id="0c899-104">Пространство имен: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0c899-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0c899-105">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="0c899-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c899-106">**Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="0c899-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c899-107">Возможные варианты настройки S режима разблокировки</span><span class="sxs-lookup"><span data-stu-id="0c899-107">The possible options to configure S mode unlock</span></span>

## <a name="members"></a><span data-ttu-id="0c899-108">Элементы</span><span class="sxs-lookup"><span data-stu-id="0c899-108">Members</span></span>
|<span data-ttu-id="0c899-109">Элемент</span><span class="sxs-lookup"><span data-stu-id="0c899-109">Member</span></span>|<span data-ttu-id="0c899-110">Значение</span><span class="sxs-lookup"><span data-stu-id="0c899-110">Value</span></span>|<span data-ttu-id="0c899-111">Описание</span><span class="sxs-lookup"><span data-stu-id="0c899-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c899-112">Ограничение</span><span class="sxs-lookup"><span data-stu-id="0c899-112">noRestriction</span></span>|<span data-ttu-id="0c899-113">нуль</span><span class="sxs-lookup"><span data-stu-id="0c899-113">0</span></span>|<span data-ttu-id="0c899-114">Этот параметр удалит все ограничения для режима разблокировки S — значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="0c899-114">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="0c899-115">блок</span><span class="sxs-lookup"><span data-stu-id="0c899-115">block</span></span>|<span data-ttu-id="0c899-116">1,1</span><span class="sxs-lookup"><span data-stu-id="0c899-116">1</span></span>|<span data-ttu-id="0c899-117">Этот параметр блокирует возможность пользователя разблокировать устройство в режиме S</span><span class="sxs-lookup"><span data-stu-id="0c899-117">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="0c899-118">блокиру</span><span class="sxs-lookup"><span data-stu-id="0c899-118">unlock</span></span>|<span data-ttu-id="0c899-119">2</span><span class="sxs-lookup"><span data-stu-id="0c899-119">2</span></span>|<span data-ttu-id="0c899-120">Этот параметр позволяет разблокировать устройство в режиме S</span><span class="sxs-lookup"><span data-stu-id="0c899-120">This option will unlock the device from S mode</span></span>|




