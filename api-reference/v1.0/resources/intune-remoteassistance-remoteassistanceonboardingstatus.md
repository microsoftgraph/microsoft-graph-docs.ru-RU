---
title: тип переименовки remoteAssistanceOnboardingStatus
description: Текущее состояние соединиттеля TeamViewer
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 04e9c73c0b0e1c6218332169bea16e3ccc2900772745008525ab1b2b031de7b8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 08/05/2021
ms.locfileid: "54182436"
---
# <a name="remoteassistanceonboardingstatus-enum-type"></a>тип переименовки remoteAssistanceOnboardingStatus

Пространство имен: microsoft.graph

> **Примечание.** API Microsoft Graph для Intune требует наличия [активной лицензии Intune](https://go.microsoft.com/fwlink/?linkid=839381) для клиента.

Текущее состояние соединиттеля TeamViewer

## <a name="members"></a>Элементы
|Элемент|Значение|Описание|
|:---|:---|:---|
|notOnboarded|0|Состояние, сообщаемое при отсутствие активного соединитетеля TeamViewer, настроенного или активного|
|onboarding|1|Состояние, сообщалось, когда система инициировала подключение TeamViewer, но служба еще не завершила подтверждение соединитетеля|
|onboarded|2|Состояние, о чем сообщалось, когда система успешно обменивалась сведениями о учетных записях с TeamViewer и теперь может инициировать сеансы удаленной помощи с клиентами|




