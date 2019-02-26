---
title: тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе
description: Возможные значения для Фиреваллпрешаредкэйенкодингмесод
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c62144ef2974da5a3d975c759bb8d2bd2be6032
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259551"
---
# <a name="firewallpresharedkeyencodingmethodtype-enum-type"></a><span data-ttu-id="f2e6b-103">тип перечисления Фиреваллпрешаредкэйенкодингмесодтипе</span><span class="sxs-lookup"><span data-stu-id="f2e6b-103">firewallPreSharedKeyEncodingMethodType enum type</span></span>

> <span data-ttu-id="f2e6b-104">**Примечание:** Для API Microsoft Graph для Intune требуется [Активная лицензия Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.</span><span class="sxs-lookup"><span data-stu-id="f2e6b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2e6b-105">Возможные значения для Фиреваллпрешаредкэйенкодингмесод</span><span class="sxs-lookup"><span data-stu-id="f2e6b-105">Possible values for firewallPreSharedKeyEncodingMethod</span></span>

## <a name="members"></a><span data-ttu-id="f2e6b-106">Элементы</span><span class="sxs-lookup"><span data-stu-id="f2e6b-106">Members</span></span>
|<span data-ttu-id="f2e6b-107">Элемент</span><span class="sxs-lookup"><span data-stu-id="f2e6b-107">Member</span></span>|<span data-ttu-id="f2e6b-108">Значение</span><span class="sxs-lookup"><span data-stu-id="f2e6b-108">Value</span></span>|<span data-ttu-id="f2e6b-109">Описание</span><span class="sxs-lookup"><span data-stu-id="f2e6b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2e6b-110">Девицедефаулт</span><span class="sxs-lookup"><span data-stu-id="f2e6b-110">deviceDefault</span></span>|<span data-ttu-id="f2e6b-111">нуль</span><span class="sxs-lookup"><span data-stu-id="f2e6b-111">0</span></span>|<span data-ttu-id="f2e6b-112">Значение не настроено Intune, не переопределять значение устройства по умолчанию, настроенное пользователем</span><span class="sxs-lookup"><span data-stu-id="f2e6b-112">No value configured by Intune, do not override the user-configured device default value</span></span>|
|<span data-ttu-id="f2e6b-113">Нет</span><span class="sxs-lookup"><span data-stu-id="f2e6b-113">none</span></span>|<span data-ttu-id="f2e6b-114">1,1</span><span class="sxs-lookup"><span data-stu-id="f2e6b-114">1</span></span>|<span data-ttu-id="f2e6b-115">Общий ключ не кодируется.</span><span class="sxs-lookup"><span data-stu-id="f2e6b-115">Preshared key is not encoded.</span></span> <span data-ttu-id="f2e6b-116">Вместо этого он хранится в расширенном формате символов</span><span class="sxs-lookup"><span data-stu-id="f2e6b-116">Instead, it is kept in its wide-character format</span></span>|
|<span data-ttu-id="f2e6b-117">utF8</span><span class="sxs-lookup"><span data-stu-id="f2e6b-117">utF8</span></span>|<span data-ttu-id="f2e6b-118">2</span><span class="sxs-lookup"><span data-stu-id="f2e6b-118">2</span></span>|<span data-ttu-id="f2e6b-119">Кодирование общего ключа с помощью UTF – 8</span><span class="sxs-lookup"><span data-stu-id="f2e6b-119">Encode the preshared key using UTF-8</span></span>|



