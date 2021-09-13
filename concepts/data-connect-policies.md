---
title: Политики и лицензирование подключения к данным Microsoft Graph
description: Описаны поддерживаемые политики и способ назначения номеров SKU для доступа независимых поставщиков программного обеспечения в организации.
author: fercobo-msft
ms.localizationpriority: high
ms.prod: data-connect
ms.openlocfilehash: 7bfff12f4ca8bb8f61f6e9e45fab3fff488ed9d6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/12/2021
ms.locfileid: "59108746"
---
# <a name="microsoft-graph-data-connect-policies-and-billing"></a>Политики и выставление счетов для подключения к данным Microsoft Graph

Подключение к данным Microsoft Graph осуществляется с помощью [управляемых приложений Azure](/azure/managed-applications/overview). С их помощью вы можете создать и развернуть решения в среде Azure. С помощью управляемых приложений вы можете поддерживать определенные политики Azure, обеспечивая клиентам более высокий доверительный уровень и комфортность при использовании приложений.

## <a name="policies"></a>Политики

Управляемые приложения Azure, созданные на основе данных Microsoft 365, поддерживают следующие политики Azure:

- [Служба хранилища Azure и требуемая политика ADLS 2-го поколения](/azure/storage/common/policy-reference)
- [Требуемая политика ADLS 1-го поколения](/azure/data-lake-store/policy-reference)

> [!NOTE]
> Azure Data Lake Store 1-го и 2-го поколения используют разные политики, так как ADLS 2-го поколения реализует службу хранилища Azure.

После проверки состояния соответствия политике, выбранной во время публикации в Azure Marketplace, она применяется ко всем установленным экземплярам приложения. Все соответствующие выбранные политики отображаются для лиц, утверждающих данные, в рамках запроса данных. В случае нарушения соответствия политике происходит сбой в работе канала и прекращается извлечение данных.

## <a name="billing-for-microsoft-graph-data-connect"></a>Выставление счетов за подключение к данным Microsoft Graph

Счет будет связан с подпиской на Azure вашей Фабрики данных Azure. Цена в этой новой модели выставления счетов зависит от количества объектов Microsoft Graph, к которым вы обращаетесь.

Эта новая возможность выставления счетов доступна в предварительной версии. Ставка составляет 0,375 долл. США за 1 000 объектов Microsoft Graph. Например, если вы обращаетесь к 10 000 объектов, вы получите счет Azure на 3,75 долл. США. По окончании действия предварительной версии ставка составит 0,75 долл. США за 1 000 объектов Microsoft Graph.

Объекты каталога, за которые не выставляются счета:

- BasicDataSet_v0.User
- BasicDataSet_v0.MailboxSettings
- BasicDataSet_v0.Manager
- BasicDataSet_v0.DirectReport

## <a name="see-also"></a>См. также

- [Политики служба хранилища Azure](/azure/storage/common/policy-reference)
- [Выставление счетов за подключение к данным Microsoft Graph](https://azure.microsoft.com/pricing/details/graph-data-connect/)
- [Управляемые приложения Azure](/azure/managed-applications/overview)
- [Выбор и фильтрация пользователей](data-connect-filtering.md)
- [Вопросы и ответы о подключении к данным](data-connect-faq.md)
