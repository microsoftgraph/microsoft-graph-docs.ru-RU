---
title: тип enum androidDeviceOwnerCrossProfileDataSharing
description: Enum, представляющий возможные значения для совместного доступа к данным из перекрестного профиля.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2e30b55d7e99e3d33914b666a2088ad29178890a
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 12/08/2021
ms.locfileid: "61348425"
---
# <a name="androiddeviceownercrossprofiledatasharing-enum-type"></a>тип enum androidDeviceOwnerCrossProfileDataSharing

Пространство имен: microsoft.graph

> **Важно:** Microsoft Graph API в /бета-версии могут изменяться; использование продукции не поддерживается.

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Enum, представляющий возможные значения для совместного доступа к данным из перекрестного профиля.

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notConfigured|0|Не настроен; это значение по умолчанию CROSS_PROFILE_DATA_SHARING_UNSPECIFIED.|
|crossProfileDataSharingBlocked|1|Данные не могут быть общими как из личного профиля в рабочий профиль, так и из профиля работы в личный профиль.|
|dataSharingFromWorkToPersonalBlocked|2|Не позволяет пользователям обмениваться данными из профиля работы с приложениями в личном профиле. Персональные данные можно использовать в приложениях для работы.|
|crossProfileDataSharingAllowed|3|Данные из любого профиля можно делиться с другим профилем.|
|unkownFutureValue|4|Неизвестное будущее значение (зарезервировано, не используется прямо сейчас)|




