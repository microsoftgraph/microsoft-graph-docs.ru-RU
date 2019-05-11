---
title: тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе
description: Возможные значения для Фиреваллпрешаредкэйенкодингмесод
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 052eb026b7668f9159d1a091c32b229b1e1bf04d
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946625"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="7a1a2-103">тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="7a1a2-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="7a1a2-104">**Важно!** API Microsoft Graph в версии/Beta могут изменяться; рабочее использование не поддерживается.</span><span class="sxs-lookup"><span data-stu-id="7a1a2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7a1a2-105">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="7a1a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7a1a2-106">Возможные значения для Фиреваллпрешаредкэйенкодингмесод</span><span class="sxs-lookup"><span data-stu-id="7a1a2-106">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="7a1a2-107">Элементы</span><span class="sxs-lookup"><span data-stu-id="7a1a2-107">Members</span></span>
|<span data-ttu-id="7a1a2-108">Элемент</span><span class="sxs-lookup"><span data-stu-id="7a1a2-108">Member</span></span>|<span data-ttu-id="7a1a2-109">Значение</span><span class="sxs-lookup"><span data-stu-id="7a1a2-109">Value</span></span>|<span data-ttu-id="7a1a2-110">Описание</span><span class="sxs-lookup"><span data-stu-id="7a1a2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7a1a2-111">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="7a1a2-111">deviceDefault</span></span>|<span data-ttu-id="7a1a2-112">нуль</span><span class="sxs-lookup"><span data-stu-id="7a1a2-112">0</span></span>|<span data-ttu-id="7a1a2-113">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="7a1a2-113">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="7a1a2-114">none</span><span class="sxs-lookup"><span data-stu-id="7a1a2-114">none</span></span>|<span data-ttu-id="7a1a2-115">1,1</span><span class="sxs-lookup"><span data-stu-id="7a1a2-115">1</span></span>|<span data-ttu-id="7a1a2-116">Общий ключ не кодируется.</span><span class="sxs-lookup"><span data-stu-id="7a1a2-116">Preshared key is not encoded.</span></span> <span data-ttu-id="7a1a2-117">Вместо этого он хранится в расширенном формате символов</span><span class="sxs-lookup"><span data-stu-id="7a1a2-117">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="7a1a2-118">utF8</span><span class="sxs-lookup"><span data-stu-id="7a1a2-118">utF8</span></span>|<span data-ttu-id="7a1a2-119">2</span><span class="sxs-lookup"><span data-stu-id="7a1a2-119">2</span></span>|<span data-ttu-id="7a1a2-120">Кодирование общего ключа с помощью UTF – 8</span><span class="sxs-lookup"><span data-stu-id="7a1a2-120">Encode the preshared key using UTF-8</span></span>|




